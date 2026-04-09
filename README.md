# Guia comandos Github

### Verificar que Git esté instalado:

git --version


### Configurar nombre y correo (una vez por computadora):

git config --global user.name "TuNombre"
git config --global user.email "tu@email.com
"


### Opcional: que Git recuerde tu token:

git config --global credential.helper store


### Crear una carpeta y entrar en ella:

mkdir ~/Documentos/MiProyecto
cd ~/Documentos/MiProyecto


### Crear un archivo, por ejemplo README.md:

nvim README.md # o nano, vim, code, lo que uses


### Inicializar Git en la carpeta:

git init


### Verificar el estado del repositorio:

git status


### Agregar todos los archivos al staging:

git add .


### Agregar un archivo específico:

git add README.md


### Hacer un commit con mensaje:

git commit -m "Primer commit: agrego README"


### Agregar un remoto (GitHub):

git remote add origin https://github.com/TuUsuario/TuRepo.git


### Verificar remoto:

git remote -v


### Subir cambios por primera vez:

git push -u origin main


### Para los siguientes commits:

git add .
git commit -m "Mensaje descriptivo"
git push


### Traer cambios del remoto:

git pull origin main


### Traer cambios sin fusionarlos automáticamente:

git fetch origin
git log HEAD..origin/main --oneline


### Ver estado e historial:

git status
git log
git log --oneline
git diff


### Trabajar con ramas:

git branch nombre_rama # crear rama
git checkout nombre_rama # cambiar de rama
git push -u origin nombre_rama # subir rama al remoto
git checkout main
git merge nombre_rama # combinar ramas


### Subir archivos o carpetas específicos:

git add archivo.md
git commit -m "Agrego archivo específico"
git push

git add carpeta/
git commit -m "Agrego carpeta con contenido"
git push


### Consejos prácticos:
- Haz commits pequeños y descriptivos.
- Organiza tus archivos en carpetas.
- Siempre haz `git pull` antes de `git push` si trabajas en repositorios compartidos.
- No compartas tu token en repos privados.

### Resumen de flujo básico:
- Crear carpeta → git init → crear archivos → git add → git commit → git remote add origin → git push
- Cambios futuros: git add → git commit → git push → git pull
