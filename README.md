# qVista

<p align="center">
  <strong>Geographic Information System (GIS) application & API built on QGIS and PyQt</strong><br>
  Developed by the Department of Territorial Information Systems — Municipal Institute of Informatics (IMI), <strong>Ajuntament de Barcelona</strong>.
</p>

<p align="center">
  <a href="#english"><img src="https://img.shields.io/badge/Language-English-blue.svg" alt="English"></a>
  <a href="#català"><img src="https://img.shields.io/badge/Llengua-Català-red.svg" alt="Català"></a>
  <a href="#castellano"><img src="https://img.shields.io/badge/Idioma-Castellano-yellow.svg" alt="Castellano"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-GPL--3.0-green.svg" alt="GPL-3.0 License"></a>
  <a href="https://qgis.org/"><img src="https://img.shields.io/badge/Powered%20by-QGIS%20API-orange.svg" alt="QGIS"></a>
</p>

---

## English

### Overview

**qVista** is an open-source desktop Geographic Information System (GIS) application and modular Python framework built on top of the **QGIS 3 API** and **PyQt5**. It provides an intuitive, high-performance environment tailored for technical services, municipal operators, and management teams.

qVista simplifies daily spatial workflows including address searching (geocoding), interactive layer and map catalogs (public, private, and local), advanced spatial printing/exporting, and custom analytical tool integration.

### Key Features

- **Intuitive Desktop Viewer**: Fast visualization, querying, and analysis of raster and vector geospatial data.
- **Barcelona Address Search Engine**: High-accuracy address and intersection search powered by local geocoding databases.
- **Multi-tiered Map & Layer Catalog**: Structured organization for shared organizational catalogs (public, restricted/departmental, and local).
- **Custom Tool Ecosystem (`moduls/eines`)**: Tools for coordinates inspection, route calculations, 3D/panoramic image viewers, buffer analysis, polygon selection, and more.
- **Extensible Python API**: Over 90 reusable PyQt/QGIS UI components and headless utilities (`moduls/Qv*.py`) for building bespoke spatial applications.
- **Custom Print & Layout Composer**: Automated high-resolution plan and atlas generation (A4, A3, A2, A1) with customizable map layouts.

### System Requirements & Installation

1. **QGIS Installation**:
   - Install **QGIS 3.10 LTR** or higher (tested on QGIS 3.22 / 3.28 / 3.34 LTR) with Python 3 bindings enabled.
   - For detailed step-by-step QGIS setup, see [guies/instalacio-qgis.md](guies/instalacio-qgis.md).

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/AjuntamentdeBarcelona/qVista.git
   cd qVista
   ```

3. **Running the Application**:
   Launch qVista using the Python environment provided with your QGIS installation:
   - **Windows** (Command prompt / Shortcut):
     ```cmd
     "C:\Program Files\QGIS 3.34\bin\python-qgis.bat" qVista.py
     ```
   - **Linux / macOS**:
     ```bash
     python3 qVista.py
     ```

4. **Configuration**:
   - Base settings are provided in `configuracioQvista_default.py`.
   - To customize paths for map catalogs, temporary folders, or database connections, create a local `configuracioQvista.py` (which is excluded by `.gitignore`).
   - For installation profiles (Production, Development, External), refer to `install.cfg` and [docs/](docs/).

### Architecture & Development

- `qVista.py`: Main application launcher.
- [moduls/](moduls/): Core library of reusable spatial widgets (`QvCanvas`, `QvLlegenda`, `QvAtributs`, etc.).
- [moduls/eines/](moduls/eines/): Modular interactive desktop tools.
- [exemples/](exemples/): Standalone examples demonstrating API usage.
- [guies/](guies/): Comprehensive technical guides and coding conventions.

### Contributing & License

- **License**: GNU General Public License v3.0 ([LICENSE](LICENSE)).
- **Contributing**: Please read [CONTRIBUTING.md](CONTRIBUTING.md) for code style guidelines and workflow recommendations.
- **Security**: See [SECURITY.md](SECURITY.md) for reporting vulnerabilities.

---

## Català

### Descripció

**qVista** és una aplicació d'escriptori de Sistemes d'Informació Geogràfica (SIG) i una llibreria modular en Python construïda sobre l'**API de QGIS 3** i **PyQt5**. Està dissenyada per simplificar l'accés i l'anàlisi de la informació territorial per a serveis tècnics, gestors municipals i ciutadania.

És un projecte impulsat pel Departament de Sistemes d'Informació Territorial de l'Institut Municipal d'Informàtica (IMI) de l'**Ajuntament de Barcelona**.

### Funcionalitats Principals

- **Visualitzador intuïtiu**: Consulta, selecció i anàlisi ràpida de capes vectorials i ràster.
- **Cercador d'adreces de Barcelona**: Geocodificació precisa d'adreces postals, cruïlles i punts d'interès.
- **Catàleg de mapes i capes en 3 nivells**: Catàleg públic compartit, catàleg privat/departamental i catàleg local.
- **Ecosistema d'eines (`moduls/eines`)**: Eines per a càlcul de rutes, visor d'imatges/panoràmiques, coordenades, filtratge per atributs i anàlisi espacial.
- **API modular**: Més de 90 components visuals i mòduls reutilitzables (`QvCanvas`, `QvLlegenda`, `QvTaulaAtributs`, etc.).
- **Impressions i plànols automàtics**: Generació de sortides gràfiques en múltiples formats (A4 a A1).

### Instal·lació i Execució

1. **Requisits previs**: Tenir instal·lat QGIS 3.10 LTR o superior (recomanat QGIS 3.28 / 3.34 LTR). Consulteu [guies/instalacio-qgis.md](guies/instalacio-qgis.md).
2. **Execució**:
   ```cmd
   "C:\Program Files\QGIS 3.34\bin\python-qgis.bat" qVista.py
   ```
3. **Configuració**: Modifiqueu o creeu el fitxer local `configuracioQvista.py` per ajustar els camins del catàleg de mapes o directoris de treball.

Per a més informació tècnica, consulteu les guies detallades a [guies/](guies/).

---

## Castellano

### Descripción

**qVista** es una aplicación de escritorio de Sistemas de Información Geográfica (SIG) y un conjunto de librerías en Python construidas sobre la **API de QGIS 3** y **PyQt5**. Está orientada a facilitar el uso y la consulta de datos geoespaciales para áreas técnicas y directivas.

Proyecto desarrollado por el Departamento de Sistemas de Información Territorial del Instituto Municipal de Informática (IMI) del **Ayuntamiento de Barcelona**.

### Características Principales

- Visualizador ágil de capas y proyectos QGIS (`.qgs` / `.qgz`).
- Buscador y geocodificador avanzado de direcciones y cruces de la ciudad de Barcelona.
- Catálogo organizado de mapas corporativos (público, privado y local).
- Módulos y herramientas personalizadas de análisis territorial y movilidad.
- Motor de impresión automatizada con plantillas de maquetación configurables.

Para instrucciones completas de instalación y desarrollo, consulte la sección en inglés o las guías en [guies/](guies/).

