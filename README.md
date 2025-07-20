
# ¿Qué tienes para mí, Sabaneta?

**¿Qué tienes para mí, Sabaneta?** es una aplicación web desarrollada con Django que permite a los usuarios descubrir negocios locales del municipio de Sabaneta según sus necesidades específicas. Además, permite a los comerciantes registrar sus negocios proporcionando información clave como sector, ubicación y redes sociales.

---

## 🚀 Características

- 🔍 Búsqueda de negocios por palabra clave o tipo de producto/servicio.
- 🏪 Registro de nuevos comercios con información relevante.
- 🧠 Recomendación de empresas basada en aprendizaje automático (scikit-learn).
- 📍 Clasificación por sectores y subsectores económicos.
- 🌐 Integración con redes sociales (Facebook e Instagram).

---

## 🛠 Tecnologías utilizadas

- **Python**: 3.13.2
- **Django**: >= 4.2
- **Pandas**: 2.0
- **scikit-learn**: 1.2
- **Openpyxl**: 3.1
- **Pillow**: 10.0
- **spaCy**: 3.8

---

## 📂 Estructura del proyecto

recomendador_sabaneta/
│
├── backend/
│ ├── manage.py
│ ├── settings.py
│ ├── urls.py
│ ├── wsgi.py
│ ├── apps/
│ │ └── recomendador/
│ │ ├── models.py
│ │ ├── forms.py
│ │ ├── views.py
│ │ ├── urls.py
│ │ └── recommender.py
│ └── pycache/
├── venv/
│ └── Scripts/
│ └── Activate.ps1
└── requirements.txt

yaml
Copiar
Editar

---

## 📝 Página de Registro de Comercios

La app incluye una interfaz accesible desde:

- **URL local**: [http://127.0.0.1:8000/registro/](http://127.0.0.1:8000/registro/)
- **Funcionalidad**:
  - Registro de nuevos negocios en el sistema.
  - Campos solicitados: nombre, sector, subsector, dirección, links de Facebook e Instagram.
  - Validación automática de URLs.
  - Almacenamiento en base de datos para usar en consultas y recomendaciones.

---

## ⚙️ Instalación y ejecución

Sigue estos pasos para ejecutar el proyecto localmente:

### 1. Clonar el repositorio

```bash
git clone https://github.com/afra7547/Recomendador-Sabaneta.git
cd Recomendador-Sabaneta/recomendador_sabaneta/backend

2. Abrir PowerShell y navegar a la carpeta del proyecto

cd "C:\Users\Pepito\Desktop\recomendador-sabaneta"

3. Crear y activar entorno virtual
bash
Copiar
Editar
# Windows
python -m venv venv
venv\Scripts\Activate.ps1

# Linux/Mac
python3 -m venv venv
source venv/bin/Activate.ps1

4. Instalar dependencias
bash
Copiar
Editar
pip install -r requirements.txt

4. Entrar a la carpeta backend en powershell
- CopiarEditar
cd ruta backend

Ejemplo: C:\Users\Soportedrai\Documents\recomendador_sabaneta\recomendador_sabaneta\backend

5. Preparar la base de datos
bash
Copiar
Editar
python manage.py makemigrations recomendador
python manage.py migrate

6. Ejecutar el servidor
bash
Copiar
Editar
python manage.py runserver
Accede a la app en tu navegador: http://127.0.0.1:8000 y http://127.0.0.1:8000/registro/

👨‍💻 Autor
Andrés Felipe Rodríguez Agudelo

Proyecto con fines sociales y educativos para promover el comercio local en Sabaneta, Antioquia (Colombia).

📄 Licencia
Este proyecto es de uso libre bajo licencia MIT. Puedes modificarlo, distribuirlo y adaptarlo con fines académicos, sociales o comunitarios.

