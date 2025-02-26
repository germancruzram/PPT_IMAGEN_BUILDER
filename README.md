# PPT_IMAGEN_BUILDER
Creador de diapostivas con imágenes


# Mapa Mental del Sistema PPT-SLIDE-BUILDER
````mermaid
graph LR
    %% Nodo central
    PPT_BUILDER(("📊 PPT-SLIDE<br>BUILDER"))
    
    %% Nodos principales (categorías)
    ProcImg{"🖼️ Procesamiento<br>de Imágenes"}
    FormatSlide{"📐 Formatos de<br>Diapositiva"}
    UI{"🖱️ Interfaz de<br>Usuario"}
    FileManage{"📁 Gestión de<br>Archivos"}
    SlideDesign{"🎨 Diseño de<br>Diapositivas"}
    Security{"🔒 Seguridad"}
    
    %% Conexiones al nodo central
    ProcImg --> PPT_BUILDER
    FormatSlide --> PPT_BUILDER
    UI --> PPT_BUILDER
    PPT_BUILDER --> FileManage
    PPT_BUILDER --> SlideDesign
    PPT_BUILDER --> Security
    
    %% Nodos secundarios para Procesamiento de Imágenes
    AspectRatio["🔍 Preservar<br>aspecto"] --> ProcImg
    Formats["📁 JPG, JPEG,<br>PNG"] --> ProcImg
    
    %% Nodos secundarios para Formatos de Diapositiva
    Standard["📏 Estándar<br>4:3"] --> FormatSlide
    Widescreen["🖥️ Panorámica<br>16:9"] --> FormatSlide
    
    %% Nodos secundarios para Interfaz de Usuario
    Tabs["📑 Pestañas"] --> UI
    Info["ℹ️ Información"] --> UI
    
    %% Nodos secundarios para Gestión de Archivos
    FolderSelect["📂 Selección<br>carpeta"] --> FileManage
    SavePPTX["💾 Guardar<br>PPTX"] --> FileManage
    
    %% Nodos secundarios para Diseño de Diapositivas
    Grid["📐 Cuadrícula<br>2x2"] --> SlideDesign
    Divider["📏 Línea<br>separadora"] --> SlideDesign
    
    %% Nodos secundarios para Seguridad
    Verification["🔑 Verificación"] --> Security
    License["📜 Licencia"] --> Security

````


## Descripción del Sistema

El sistema PPT-SLIDE-BUILDER es una herramienta especializada para la creación automática de presentaciones de PowerPoint a partir de imágenes. El mapa mental anterior muestra los principales componentes y funcionalidades del sistema basados en el código AGENTE.PY.

### Componentes Principales

1. **Procesamiento de Imágenes**
   - Preservación de la relación de aspecto de las imágenes
   - Soporte para formatos JPG, JPEG y PNG

2. **Formatos de Diapositiva**
   - Soporte para formato estándar 4:3
   - Soporte para formato panorámico 16:9

3. **Interfaz de Usuario**
   - Sistema de pestañas para organización
   - Pestaña de información descriptiva

4. **Gestión de Archivos**
   - Selección de carpeta de imágenes
   - Guardado de archivos PowerPoint

5. **Diseño de Diapositivas**
   - Organización en cuadrícula 2x2 (4 imágenes por diapositiva)
   - Línea separadora para el membrete

6. **Seguridad**
   - Sistema de verificación de licencia
   - Gestión de archivos de licencia

