# Mi CV en LaTeX
Este repositorio contiene el código fuente de mi CV escrito en LaTeX y desplegado automáticamente con GitHub Actions y Vercel.

### Archivo principal

main.tex: Documento principal en LaTeX que define el diseño y contenido de mi CV.

### Automatización con GitHub Actions

Cada vez que se hace un commit a la rama main:

GitHub Actions compila main.tex usando pdflatex

El PDF generado se guarda como public/CV.pdf

El archivo PDF se commitea de vuelta al repositorio automáticamente

Workflow: .github/workflows/build.yml

**Incluye:**

Instalación de paquetes LaTeX necesarios (como fontawesome5, xcolor, etc.)

Compilación no interactiva con manejo de errores

Renombrado a CV.pdf

Commit automático usando github-actions[bot]

### Despliegue con Vercel

El PDF final se encuentra disponible en la URL:

https://cv-mu-steel.vercel.app

Vercel está configurado para servir la carpeta public/ donde se encuentra el PDF generado.



