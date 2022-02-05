# Instalar en Microsoft Windows ™

Descargue el último **archivo de Windows** de [versiones de QOwnNotes en GitHub](https://github.com/pbek/QOwnNotes/releases) y descomprímalo en cualquier lugar que desee. ¡No se necesita instalación!

::: advertencia Si desea utilizar el **actualizador automático**, asegúrese de descomprimirlo en un lugar donde su cuenta de usuario tenga acceso de escritura. De forma predeterminada, es muy probable que su cuenta de usuario **no tenga acceso de escritura** a lugares como `C:\Archivos de programa (x86)` o `C:\Archivos de programa`.
:::

Luego, puede ejecutar directamente `QOwnNotes.exe` desde su carpeta `QOwnNotes`, no se requiere instalación.

### Modo portátil

Utilice `QOwnNotesPortable.bat` para ejecutar QOwnNotes en **modo portátil** donde todo (incluidas sus notas) solo se almacenará en su carpeta `QOwnNotes`.

::: tip
No necesita el modo portátil si simplemente no tiene permisos de administración en su computadora. ¡No es necesario instalar QOwnNotes!
:::

## Windows XP

Qt eliminó el soporte para Windows XP con la versión 5.8, pero QOwnNotes ahora también está construido con Qt 5.7 para permitir que los usuarios de Windows XP aún lo usen.

Aunque debe buscar la última compilación maestra de [AppVeyor](https://ci.appveyor.com/project/pbek/qownnotes/history) usted mismo, elija el *entorno Qt 5.7* y descargue el *artefacto*.

::: tip Info
¡El mecanismo de actualización automática no funciona con la compilación de AppVeyor para Windows XP! Tendrá que descargar las nuevas versiones usted mismo.
:::

## Chocolatey

Hay un paquete de QOwnNotes mantenido por la comunidad en [Chocolatey](https://chocolatey.org/packages/qownnotes/).

Puedes instalarlo con:

```shell
choco install qownnotes
```

## Scoop

There is a [community maintained package of QOwnNotes](https://github.com/ScoopInstaller/Extras/blob/master/bucket/qownnotes.json) at [Scoop](https://scoop.sh/). If you add the Extras bucket you can use it to install QOwnNotes in portable mode.

```shell
scoop bucket add extras
scoop update
scoop install qownnotes
```
