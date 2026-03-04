[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/SoySH/CertMaker)

## 🖥 Compilación desde código fuente

### Windows

1. **Instalar Python** 3.13+ y marcar la opción **"Add Python to PATH"** durante la instalación.
   
2. Crear carpeta del proyecto: mkdir CertMaker
   
3. Crear un archivo llamado `app.py` con el código fuente (quitar la extensión `.txt` si la tiene).

4. Descargar un icono en formato `.ico` desde:
- [Ionicons](https://ionic.io/ionicons)  
- [Icon-icons](https://icon-icons.com/)  
- Convertirlo con [ConvertICO](https://convertico.com/icon-resizer/) **MULTIRESOLUCIÓN** (256px y 128px) y guardarlo junto a `app.py` como `ico.ico`.
5. Abrir la terminal (CMD o PowerShell) en la misma ruta. Si usas PowerShell como predeterminado, escribe: cmd y presiona **Enter** para cambiar a CMD.

6. Ejecutar:
   
- python -m venv .venv
- .venv\Scripts\activate
- pip install --upgrade pip
- pip install PyQt5 cryptography pyinstaller
- pyinstaller --onefile --windowed --icon=ico.ico --name=CertMaker app.py

7. Localiza el .exe en la carpeta dist

