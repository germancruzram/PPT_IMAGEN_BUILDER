# PPT_IMAGEN_BUILDER
Creador de diapostivas con imágenes


# Mapa Mental del Sistema PPT-SLIDE-BUILDER

graph LR
    %% Título central
    PPT_BUILDER(("📊 PPT-SLIDE\nBUILDER"))

    %% Ramas principales hacia la izquierda
    ProcImg{"🖼️ Procesamiento\nde Imágenes"} --> PPT_BUILDER
    FormatSlide{"📐 Formatos de\nDiapositiva"} --> PPT_BUILDER
    UI{"🖱️ Interfaz de\nUsuario"} --> PPT_BUILDER

    %% Ramas principales hacia la derecha
    PPT_BUILDER --> FileManage{"📁 Gestión de\nArchivos"}
    PPT_BUILDER --> SlideDesign{"🎨 Diseño de\nDiapositivas"}
    PPT_BUILDER --> Security{"🔒 Seguridad"}

    %% Subramas de Procesamiento de Imágenes (2do nivel)
    AspectRatio["🔍 Preservar\naspecto"] --> ProcImg
    Formats["📁 JPG, JPEG,\nPNG"] --> ProcImg

    %% Subramas de Formatos de Diapositiva (2do nivel)
    Standard["📏 Estándar\n4:3"] --> FormatSlide
    Widescreen["🖥️ Panorámica\n16:9"] --> FormatSlide

    %% Subramas de Interfaz de Usuario (2do nivel)
    Tabs["📑 Pestañas"] --> UI
    Info["ℹ️ Información"] --> UI

    %% Subramas de Gestión de Archivos (2do nivel)
    FolderSelect["📂 Selección\ncarpeta"] --> FileManage
    SavePPTX["💾 Guardar\nPPTX"] --> FileManage

    %% Subramas de Diseño de Diapositivas (2do nivel)
    Grid["📐 Cuadrícula\n2x2"] --> SlideDesign
    Divider["📏 Línea\nseparadora"] --> SlideDesign

    %% Subramas de Seguridad (2do nivel)
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

    %% Configuración de enlaces
    linkStyle default stroke:#666,stroke-width:2px;


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

