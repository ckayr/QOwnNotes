# Áttekintés

<template>
<v-carousel cycle show-arrows-on-hover>
  <v-carousel-item>
    <img src="/screenshots/screenshot.png" alt="QOwnNotes képernyőkép" />
    <div class="sheet">
      Szerkesztheti jegyzeteit kiemeléssel, színes címkékkel és almappákkal
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-minimal.png" alt="Minimális nézet" />
    <div class="sheet">
      Minimális alapértelmezett felhasználói felület, amely még jobban lehúzható
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-vertical.png" alt="Függőleges nézet" />
    <div class="sheet">
      Tekintse meg a jegyzeteket függőleges jelölési nézetben a panelek mozgatásával
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-portable-mode.png" alt="Hordozható üzemmód" />
    <div class="sheet">
      Hordozható mód USB-meghajtókhoz
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-1col.png" alt="Egy oszlop" />
    <div class="sheet">
      Minden panel elhelyezhető, ahová csak szeretné
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-darkmode.png" alt="screenshot darkmode" />
    <div class="sheet">
      Sötét stílus
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-distraction-free-mode.png" alt="screenshot-distraction-free-mode" />
    <div class="sheet">
      Figyelemelterelésmentes mód
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-encrypted-note-decrypted.png" alt="Jegyzet titkosítása" />
    <div class="sheet">
      Opcionális AES jegyzet titkosítás (szkriptelhető is)
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-encrypted-note.png" alt="Titkosított jegyzet" />
    <div class="sheet">
      A titkosított jegyzetek továbbra is szövegek
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-diff.png" alt="screenshot diff" />
    <div class="sheet">
      Mutassa meg a különbséget a jegyzetek között, amikor azokat külsőleg módosították
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-export-print.png" alt="screenshot-export-print" />
    <div class="sheet">
      Megjegyzés: PDF export és nyomtatás
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-freedesktop-theme.png" alt="screenshot-freedesktop-theme" />
    <div class="sheet">
      Icons via Freedesktop theme
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-other-workspace.png" alt="screenshot-other-workspace" />
    <div class="sheet">
      Különböző munkaterületei lehetnek
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-qml.png" alt="screenshot-qml" />
    <div class="sheet">
      Scriptable
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-russian.png" alt="screenshot-russian" />
    <div class="sheet">
      Sok nyelvre van lefordítva
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-search-in-all-notes.png" alt="screenshot-search-in-all-notes" />
    <div class="sheet">
      Keresés az összes jegyzet között
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-search-in-current-note.png" alt="screenshot-search-in-current-note" />
    <div class="sheet">
      Search in the current note
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-settings-note-folders.png" alt="screenshot-settings-note-folders" />
    <div class="sheet">
      Able to use multiple note folders
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-todo.png" alt="screenshot-todo" />
    <div class="sheet">
      Manage your Todo lists via CalDAV
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-trash.png" alt="screenshot-trash" />
    <div class="sheet">
      Kukázott jegyzetek kezelése a Nextcloud szerveren
    </div>
  </v-carousel-item>
  <v-carousel-item>
    <img src="/screenshots/screenshot-versioning.png" alt="screenshot-versioning" />
    <div class="sheet">
      A jegyzet verzióinak kezelése a Nextcloud szerveren
    </div>
  </v-carousel-item>
</v-carousel>
</template>

<v-divider />

**Q** a [Qt framework](https://www.qt.io/), amelyet használ  
**Own** mert birtokolja a jegyzeteit   
**Notes** az Ön jegyzetei végett, melyeket elkészít

<v-divider />

A [QOwnNotes](https://www.qownnotes.org/) a **nyílt forráskódú** (GPL) sima szövegű fájl **macOS** és **Windows**, amelyek (opcionálisan) együtt működnek a [Nextcloud](https://nextcloud.com/) és az [ownCloud](https://owncloud.org/) [**Notes alkalmazással**](https://github.com/nextcloud/notes).

::: tip
Csatlakozzon a [Telegram csoport](https://t.me/QOwnNotes)unkhoz, beszélgetés, tanulás és egymással kapcsolatba lépésünk érdekében a QOwnNotes közösséggel.
:::

[Értse meg a QOwnNotes fogalmát](concept.md)

## Funkciók
- Használhatja a **meglévő szöveges vagy jelölőfájljait**, legtöbbször nincs szükség importálásra
- A QOwnNotes C++ nyelven íródott, és **alacsony erőforrás-fogyasztásra** van optimalizálva (nincs CPU és memóriaéhes Electron alkalmazás)
- **Evernote és Joplin import**
- **Kompatibilis** a **Nextcloud / ownCloud** és a **mobile** és a Nextcloud Text Notes alkalmazásával
- Támogatás a **jegyzetek megosztásához** a **ownCloud** / **Nextcloud** kiszolgálón
- A Nextcloud / ownCloud **témalistáinak kezelése** (**Nextcloud-feladatok** vagy **Tasks Plus** / **Calendar Plus**) vagy használjon egy másik **CalDAV szervert** a feladatok szinkronizálásához
- A jegyzetek régebbi **verziói** **visszaállíthatók** a **Nextcloud / ownCloud** szerverről
- **A kukába helyezett jegyzetek** **visszaállíthatók** a **Nextcloud / ownCloud** szerverről
- A jegyzetfájlok **külső változásai** ** figyelésre kerülnek** (a jegyzetek vagy a jegyzetlista újratöltődnek)
- A **hierarchikus jegyzetcímkézés** és a **jegyzetmappák** támogatása
- Opcionális jegyzetek **titkosítása** (beépített AES-256 vagy használhat egyedi titkosítási módszereket, például **[Keybase.io](https://keybase.io/)** ([encryption-keybase.qml](https://github.com/pbek/QOwnNotes/blob/develop/doc/scripting/encryption-keybase.qml)) vagy **PGP** ([titkosítás-pgp.qml](https://github.com/pbek/QOwnNotes/blob/develop/doc/scripting/encryption-pgp.qml))
- A **jegyzetek mappa** **szabadon választható** (több jegyzetmappa is használható)
- A jegyzetek **alsztring keresése** lehetséges, és a keresési eredmények kiemelésre kerülnek a jegyzetekben
- [**Estensione del browser**](browser-extension.md) per **aggiungere note dal testo selezionato**, **fare screenshot** o **gestire i tuoi segnalibri**
- [**Helyesírás-ellenőrzés**](../editor/spellchecking.md) támogatás
- **Hordozható mód** a QOwnNotes hordozásához USB-meghajtókon
- **A szkriptek támogatása** és az online [**szkripttár**](https://github.com/qownnotes/scripts), ahol parancsfájlokat telepíthet az alkalmazásba
- **Vim mód**
- [Webalkalmazás](web-app.md) a **fényképek beillesztéséhez a mobiltelefonról** az asztali QOwnNotes aktuális jegyzetébe


## Megjelenés
- A jegyzetek **jelölésének kiemelése** és egy **jelölés előnézeti mód**
- **Sötét módú téma támogatás**
- **Támogatás** a **jelölés szintaxis kiemeléséhez**
- Minden **panel tetszőlegesen elhelyezhető**, akár **lebeghet** vagy **teljesen dokkolható**
- Támogatja a **freedesktop téma ikonokat**, használhatja a QOwnNotes programot a **natív asztali ikonokkal** és a kedvenc **sötét asztali témájával**
- **Figyelemelterelés mentes mód**, **teljes képernyős mód** és **Írógép mód**
- **Sorszám**
- **Az aktuális és a külsőleg megváltozott jegyzet közötti különbségeket** egy párbeszédpanelen **mutatják**

## Nyelvek
- **Több mint 60 különböző nyelven érhető el**, mint például angol, német, francia, lengyel, kínai, japán, orosz, portugál, magyar, holland és spanyol
  - [Segítségét](../contributing/translation.md) nagyra értékelik ezen fordítások fejlesztése vagy a QOwnNotes több nyelvre történő lefordítása érdekében

<style>
.sheet {
  position: absolute;
  bottom: 50px;
  background-color: rgba(0,0,0, 0.5);
  color: white;
  text-align: center;
  display: flex;
  align-items:center;
  justify-content:center;
  height: 50px;
  width: 100%;
}

.v-window__next {
  right: 0;
}

@media (max-width: 500px) {
  .v-carousel {
    height: 400px!important;
  }
}

@media (max-width: 350px) {
  .v-carousel {
    height: 250px!important;
  }
}

@media (max-width: 200px) {
  .v-carousel {
    height: 150px!important;
  }
}
</style>
