# Documentación de Aplicación con PySide6

## Introducción
Este proyecto es una aplicación simple de "Hola Mundo" utilizando PySide6. La documentación proporciona instrucciones detalladas para la instalación y ejecución en Windows y Linux.

## Prerrequisitos
Asegúrate de tener instalado **Python 3** en tu sistema.
Puedes verificarlo con el siguiente comando:

```sh
python --version  # o python3 --version en Linux
```

Si no está instalado, descárgalo desde [python.org](https://www.python.org/downloads/).

---

## Instalación y Configuración

### 1. Instalación de Python y pip
**Windows:**
- Descarga e instala Python desde [python.org](https://www.python.org/downloads/).
- Asegúrate de marcar la opción **"Add Python to PATH"** durante la instalación.
- Verifica la instalación:

```sh
python --version
pip --version
```

**Linux:**
- Instala Python y pip con:

```sh
sudo apt update
sudo apt install python3 python3-pip
```

---

### 2. Creación y Activación del Entorno Virtual
Es recomendable usar un entorno virtual para gestionar las dependencias del proyecto.

**Windows:**
```sh
python -m venv venv
venv\Scripts\activate
```

**Linux:**
```sh
python3 -m venv venv
source venv/bin/activate
```

---

### 3. Instalación de Dependencias
Instala PySide6 dentro del entorno virtual:

```sh
pip install PySide6
```

---

### 4. Creación del Archivo `main.py`
Crea un archivo `main.py` y copia el siguiente código:

```python
import sys
from PySide6.QtWidgets import QApplication, QLabel

app = QApplication(sys.argv)
label = QLabel("Hola Mundo")
label.show()
sys.exit(app.exec())
```

---

### 5. Ejecución de la Aplicación
Para ejecutar la aplicación, usa el siguiente comando dentro del entorno virtual:

```sh
python main.py
```

---

## Notas Adicionales
- Si tienes problemas con PySide6, intenta actualizar `pip`:

```sh
pip install --upgrade pip
```

- Para salir del entorno virtual:
  - **Windows:** `deactivate`
  - **Linux:** `deactivate`

---

## Licencia
Este proyecto se distribuye bajo la licencia MIT.

