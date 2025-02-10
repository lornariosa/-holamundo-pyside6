# Documentar Aplicación - HolaMundo en PySide6

## Instalación de Python3
### Windows:
- Descarga Python desde [python.org](https://www.python.org/downloads/).
- Verifica la instalación con:
  ```sh
  python --version
  ```

### Linux:
- Instala Python con:
  ```sh
  sudo apt update
  sudo apt install python3
  ```
- Verifica la instalación con:
  ```sh
  python3 --version
  ```



## Instalación y Activación de pip
### Windows:
- Pip ya viene incluido con Python, para asegurarte de que esté actualizado usaremos el comando:
  ```sh
  python -m pip install --upgrade pip
  ```

### Linux:
- Instalación de pip:
  ```sh
  sudo apt install python3-pip
  ```
- Verificamos la instalación con:
  ```sh
  pip3 --version
  ```



## Creación y Activación de Entorno Virtual
### Windows:
```sh
python -m venv venv
venv\Scripts\activate
```

### Linux:
```sh
python3 -m venv venv
source venv/bin/activate
```



## Instalación de Dependencias
Con el entorno virtual activado, instala PySide6:
```sh
pip install PySide6
```



## Ejecución de la Aplicación
Crea un archivo `main.py` y copia el siguiente código:

```python
import sys
from PySide6.QtWidgets import QApplication, QLabel

app = QApplication(sys.argv)
label = QLabel("Hola Mundo")
label.show()
sys.exit(app.exec())
```

Ejecuta la aplicación con:
```sh
python main.py
```
