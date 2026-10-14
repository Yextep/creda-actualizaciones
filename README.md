# Creda · actualizaciones

Creda, la app de préstamos de Daniel Lezcano (Yextep), consulta `version.json` cada vez que se abre con conexión a internet. Sin conexión funciona igual.

| Campo | Efecto en las instalaciones |
| --- | --- |
| `version`, `codigo` | Última versión publicada. Si `codigo` es mayor que el de la instalación, aparece «Actualización disponible» con **Actualizar** y **Más tarde**. |
| `apk` | Enlace de descarga (https) de esa versión. |
| `codigo_minimo` | Las instalaciones con un código menor dejan de funcionar hasta actualizar. Solo pueden exportar sus datos. |
| `bloqueada` | `true` desactiva todas las instalaciones y muestra `mensaje`. Solo pueden exportar sus datos. |

Este repositorio debe seguir siendo público y conservar este nombre: es la dirección fija que consultan las apps instaladas. Los cambios se hacen con `scripts/publicar_version.py` del proyecto de Creda o editando `version.json` aquí.
