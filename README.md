# Programa de Desarrollo eCrew (eCDP) - Traducción al ESPAÑOL

Este es un repositorio para crear un parche de traducción al español (realizado por fans) del [Programa de Desarrollo eCrew](https://en.wikipedia.org/wiki/ECrew_Development_Program) de McDonald's.

## Estructura del Repositorio

El repositorio consta de 4 secciones, una carpeta por cada sección:
- `arm9` - Traduce las secciones ARM9.
- `overlay` - Traduce los archivos overlay, que contienen textos de la interfaz de usuario, así como el código compilado del juego.
- `bin` - Traduce archivos bin, que contienen principalmente textos para las guías SOC y el Auto-chequeo.
- `cmcd` - Traduce la sección "Desafía a McDonald's". También reemplaza la fuente utilizada en esa sección.

## Parchear tu ROM

Esta guía es para aplicar todos los parches de traducción a tu ROM. Para aplicar parches a secciones individuales, consulta las instrucciones dentro de cada carpeta correspondiente.

1. Instala Python 3.9 en tu ordenador e instala el paquete `ndspy`:
   ```bash
   pip install ndspy
   ```
2. Coloca una ROM original y sin modificar del eCDP de McDonald's en este directorio. (SHA-1 del archivo: `136aacc9d3d7c8567381cd4e735ff3c004a018d0`)
3. Ejecuta `patch_all.py` con Python 3.9 (no se ha probado con otras versiones), especificando el archivo de la ROM:
   ```bash
   python patch_all.py <NombreDelArchivo>.nds
   ```
4. El script aplicará los parches de texto en todas las secciones y creará un archivo llamado `\<NombreDelArchivo\>-patched.nds`.
5. ¡Parcheado completo! Ahora puedes jugar al juego en el emulador de Nintendo DS que prefieras.
