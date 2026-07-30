# BIA Governance — Releases

Distribución oficial de la aplicación de escritorio de **BIA Governance**: la plataforma de gobierno corporativo que prepara, graba y documenta las sesiones de órganos de gobierno procesando el audio, la transcripción y las actas en local.

La última versión está siempre disponible en la [página de releases](https://github.com/Team-BIA/bia-governance-releases/releases/latest) y en [biagovernance.com/descargar](https://biagovernance.com/descargar).

## Plataformas

| Plataforma | Archivo | Requisitos |
| --- | --- | --- |
| macOS (Apple Silicon) | `BIA-Governance-<versión>-arm64.dmg` | macOS 14 o superior, chip M1 o posterior |
| Windows (x64) | `BIA-Governance-Setup-<versión>-x64.exe` | Windows 10 u 11 de 64 bits |

Los modelos de IA locales no van dentro del instalador: la aplicación los descarga de forma guiada tras la instalación, una sola vez por equipo.

## Primer arranque

Comportamiento estándar del sistema con software distribuido fuera de las tiendas:

- **macOS**: si el primer arranque queda bloqueado, abre **Ajustes del Sistema → Privacidad y seguridad** y pulsa **«Abrir igualmente»**. Solo hace falta una vez.
- **Windows**: si aparece SmartScreen, pulsa **«Más información»** y después **«Ejecutar de todas formas»**.

## Verificación

Cada release publica un `checksums.txt` con la suma SHA-256 de sus archivos. Para comprobarla:

```
# macOS
shasum -a 256 BIA-Governance-<versión>-arm64.dmg

# Windows
certutil -hashfile BIA-Governance-Setup-<versión>-x64.exe SHA256
```

## Contacto

¿Quieres verla en funcionamiento sobre un caso real? Solicita una demo en [biagovernance.com/solicitar-demo](https://biagovernance.com/solicitar-demo).
