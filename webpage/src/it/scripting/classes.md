# Classi esposte

Nota
----

### Proprietà e metodi
```cpp
class NoteApi {
    Q_PROPERTY(int id)
    Q_PROPERTY(QString name)
    Q_PROPERTY(QString fileName)
    Q_PROPERTY(QString fullNoteFilePath)
    Q_PROPERTY(QString fullNoteFileDirPath)
    Q_PROPERTY(QString relativeNoteFileDirPath)
    Q_PROPERTY(int noteSubFolderId)
    Q_PROPERTY(QString noteText)
    Q_PROPERTY(QString decryptedNoteText)
    Q_PROPERTY(bool hasDirtyData)
    Q_PROPERTY(QQmlListProperty<TagApi> tags)
    Q_PROPERTY(QDateTime fileCreated)
    Q_PROPERTY(QDateTime fileLastModified)
    Q_INVOKABLE QStringList tagNames()
    Q_INVOKABLE bool addTag(QString tagName)
    Q_INVOKABLE bool removeTag(QString tagName)
    Q_INVOKABLE bool renameNoteFile(QString newName)
    Q_INVOKABLE QString toMarkdownHtml(bool forExport = true)
    Q_INVOKABLE QString getFileURLFromFileName(QString localFileName)
    Q_INVOKABLE bool allowDifferentFileName()
};
```

Puoi usare i metodi di [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) per lavorare con `fileCreated` o `fileLastModified`.

### Esempio
```js
script.log(note.fileCreated.toISOString());
script.log(note.fileLastModified.getFullYear());

// rinomina una nota in "new name.md"
note.renameNoteFile("new name");

// controlla se è possibile avere un nome di file diverso dal titolo
script.log(note.allowDifferentFileName());
```

NoteSubFolder
----

### Proprietà e metodi
```cpp
class NoteSubFolderApi {
    Q_PROPERTY(int id)
    Q_PROPERTY(QString name)
    Q_PROPERTY(QQmlListProperty<NoteApi> notes)
    Q_INVOKABLE static NoteSubFolderApi *fetchNoteSubFolderById(int id);
    Q_INVOKABLE static QList<QObject*> fetchNoteSubFoldersByParentId(int parentId);
};
```

### Esempio
```js
script.log(noteSubFolder.id);
script.log(noteSubFolder.name);

// esegui un ciclo su tutte le note nella sottocartella note
for (var idx in noteSubFolder.notes) {
    var note = noteSubFolder.notes[idx];
}

// stampa i nomi di tutte le sottocartelle
noteSubFolder.fetchNoteSubFoldersByParentId(parentId).forEach(function(nsf) {
    script.log(nsf.name);
});
```

Etichetta (Tag)
---

### Proprietà e metodi
```cpp
class TagApi {
    Q_PROPERTY(int id)
    Q_PROPERTY(QString name)
    Q_PROPERTY(int parentId)
    Q_INVOKABLE TagApi fetchByName(const QString &name, int parentId = 0)
    Q_INVOKABLE QStringList getParentTagNames()
};
```

MainWindow
----------

### Proprietà e metodi
```cpp
class MainWindow {
    Q_INVOKABLE void reloadTagTree();
    Q_INVOKABLE void reloadNoteSubFolderTree();
    Q_INVOKABLE void buildNotesIndexAndLoadNoteDirectoryList(
            bool forceBuild = false, bool forceLoad = false);
    Q_INVOKABLE void focusNoteTextEdit();
    // Crea una nuova sottocartella note nella sottocartella corrente
    Q_INVOKABLE bool createNewNoteSubFolder(QString folderName = "");
    // Inserisce HTML nella nota corrente come markdown
    // Questo metodo scarica anche le immagini remote e trasforma
    // "data:image" URL in immagini locali memorizzate nella cartella
    // media
    Q_INVOKABLE void insertHtmlAsMarkdownIntoCurrentNote(QString html);
    // Ricarica la nota corrente per id
    // Questo viene utile quando il percorso o il nome del file della
    // nota corrente sono cambiati
    Q_INVOKABLE void reloadCurrentNoteByNoteId();
    // Restituisce gli UUID degli spazi di lavoro
    Q_INVOKABLE QStringList getWorkspaceUuidList();
    // Restituisce l'UUID di uno spazio di lavoro, passandogli il nome
    // dello spazio di lavoro
    Q_INVOKABLE QString getWorkspaceUuid(const QString &workspaceName);
    // Imposta lo spazio di lavoro corrente tramite UUID
    Q_INVOKABLE void setCurrentWorkspace(const QString &uuid);
};
```

### Esempio
```js
// Forza il caricamento della lista note
mainWindow.buildNotesIndexAndLoadNoteDirectoryList(true, true);

// Crea una nuova  sottocartella note "My fancy folder" nella sottocartella corrente
mainWindow.createNewNoteSubFolder("My fancy folder");

// Inserisce HTML nella nota corrente come markdown
mainWindow.insertHtmlAsMarkdownIntoCurrentNote("<h2>my headline</h2>some text");

// Imposta lo spazio di lavoro 'Edit' come spazio di lavoro corrente
mainWindow.setCurrentWorkspace(mainWindow.getWorkspaceUuid("Edit"));
```
