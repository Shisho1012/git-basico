# Guía de comandos básicos de Git

## Preparar cambios
- `git add .` → agrega todos los cambios al staging
- `git add <archivo>` → agrega un archivo específico

## Guardar cambios
- `git commit -m "mensaje"` → guarda cambios localmente

## Sincronización con GitHub
- `git push origin main` → sube commits locales al repo remoto
- `git pull origin main` → trae cambios del repo remoto a local

## Ver estado
- `git status` → muestra archivos modificados, agregados o sin seguimiento
- `git log` → muestra el historial de commits

## Configuración
- `git config --global user.name "TuNombre"` → define autor
- `git config --global user.email "tu@email.com"` → define email
# Opcional: que Git recuerde tu token para no pedirlo cada vez
git config --global credential.helper store

# Crear repo local en la carpeta actual
git init

# Verifica que esté creado
git status

# Agrega el repo remoto (origin)
git remote add origin https://github.com/Shisho1012/Cisco-Networks.git

# Verifica que se agregó
git remote -v

# Agrega todos los archivos y carpetas del repo
git add .

# O agrega un archivo específico
git add Guia-Git.md
git add temas/1_Introduccion.md

# Crea un commit con mensaje
git commit -m "Primer commit: estructura inicial del curso"

# Crear otro commit más adelante
git commit -m "Agrego guía de comandos de Git

# Primera vez que subes una rama principal
git push -u origin main

# Después solo necesitas
git push

# Actualiza tu repo local con cambios del remoto
git pull origin main

# Ver los commits que existen en remoto pero no en local
git fetch origin
git log HEAD..origin/main --oneline

git status       # Archivos modificados, agregados o sin seguimiento
git log          # Historial de commits
git log --oneline  # Versión resumida del historial
git diff         # Diferencias de archivos modificados

# Crear nueva rama
git branch nombre_rama

# Cambiar de rama
git checkout nombre_rama

# Subir rama al remoto
git push -u origin nombre_rama


