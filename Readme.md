## CV Wilmar Sepulveda 2024

Este proyecto contiene el código LaTeX que genera mi Hoja de vida actualizada en formato PDF.

### Estructura del Proyecto

```
cv_wilmar_latex/
├── common/                    # Archivos compartidos entre versiones
│   ├── preamble.tex          # Preámbulo común (paquetes, configuración)
│   ├── commands.tex           # Comandos personalizados compartidos
│   ├── sections.tex          # Estructura de secciones común
│   ├── titles-en.tex         # Títulos de secciones en inglés
│   └── titles-es.tex         # Títulos de secciones en español
├── english/                   # Versión en inglés
│   ├── main.tex              # Archivo principal (usa archivos comunes)
│   └── particulars.tex       # Contenido específico en inglés
├── spanish/                   # Versión en español
│   ├── main.tex              # Archivo principal (usa archivos comunes)
│   └── particulars.tex      # Contenido específico en español
├── logos/                     # Logos de tecnologías
└── utilities.tex              # Plantillas para educación, experiencia, proyectos
```

### Cómo compilar

Para compilar el CV en inglés:
```bash
cd english
pdflatex main.tex
```

Para compilar el CV en español:
```bash
cd spanish
pdflatex main.tex
```

### Ventajas de la estructura modular

- **Sin duplicación**: El código común está centralizado en `common/`
- **Fácil mantenimiento**: Cambios en formato se hacen una sola vez
- **Separación de idiomas**: Solo los títulos y contenido cambian por idioma
- **Escalable**: Fácil agregar nuevos idiomas o secciones
