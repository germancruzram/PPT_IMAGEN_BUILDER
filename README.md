# PPT_IMAGEN_BUILDER
Creador de diapostivas con imágenes


# Mapa Mental del Sistema PPT-SLIDE-BUILDER
flowchart TD
    %% Nodo central
    PPT_BUILDER(("📊 PPT-SLIDE\nBUILDER"))
    
    %% Nodos principales (categorías)
    ProcImg{"🖼️ Procesamiento\nde Imágenes"}
    FormatSlide{"📐 Formatos de\nDiapositiva"}
    UI{"🖱️ Interfaz de\nUsuario"}
    FileManage{"📁 Gestión de\nArchivos"}
    SlideDesign{"🎨 Diseño de\nDiapositivas"}
    Security{"🔒 Seguridad"}
    
    %% Conexiones al nodo central
    ProcImg --> PPT_BUILDER
    FormatSlide --> PPT_BUILDER
    UI --> PPT_BUILDER
    PPT_BUILDER --> FileManage
    PPT_BUILDER --> SlideDesign
    PPT_BUILDER --> Security
    
    %% Nodos secundarios para Procesamiento de Imágenes
    AspectRatio["🔍 Preservar\naspecto"] --> ProcImg
    Formats["📁 JPG, JPEG,\nPNG"] --> ProcImg
    
    %% Nodos secundarios para Formatos de Diapositiva
    Standard["📏 Estándar\n4:3"] --> FormatSlide
    Widescreen["🖥️ Panorámica\n16:9"] --> FormatSlide
    
    %% Nodos secundarios para Interfaz de Usuario
    Tabs["📑 Pestañas"] --> UI
    Info["ℹ️ Información"] --> UI
    
    %% Nodos secundarios para Gestión de Archivos
    FolderSelect["📂 Selección\ncarpeta"] --> FileManage
    SavePPTX["💾 Guardar\nPPTX"] --> FileManage
    
    %% Nodos secundarios para Diseño de Diapositivas
    Grid["📐 Cuadrícula\n2x2"] --> SlideDesign
    Divider["📏 Línea\nseparadora"] --> SlideDesign
    
    %% Nodos secundarios para Seguridad
    Verification["🔑 Verificación"] --> Security
    License["📜 Licencia"] --> Security
    
    %% Estilos
    classDef default fill:#f9f9f9,stroke:#333,stroke-width:1px;
    classDef central fill:#4285F4,color:#fff,stroke:#2171C7,stroke-width:3px;
    classDef primary fill:#5DADE2,color:#fff,stroke:#2E86C1,stroke-width:2px;
    classDef secondary fill:#E8F4F8,stroke:#AED6F1,stroke-width:1px;
    
    %% Aplicación de estilos
    class PPT_BUILDER central;
    class ProcImg,FormatSlide,UI,FileManage,SlideDesign,Security primary;
    class AspectRatio,Formats,Standard,Widescreen,Tabs,Info,FolderSelect,SavePPTX,Grid,Divider,Verification,License secondary;



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

