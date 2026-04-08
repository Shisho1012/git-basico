Guía completa de Git y GitHub
1️⃣ Preparación inicial

Antes de usar Git:

Verifica que Git esté instalado:
git --version
Configura tu identidad (una sola vez por computadora):
git config --global user.name "TuNombre"
git config --global user.email "tu@email.com"
Esto identifica quién hace los commits.
Opcional: que Git recuerde tu contraseña/token:
git config --global credential.helper store
2️⃣ Crear un archivo y un repositorio local
Crea una carpeta para tu proyecto:
mkdir ~/Documentos/MiProyecto
cd ~/Documentos/MiProyecto
Crea un archivo, por ejemplo README.md:
nvim README.md   # o nano, vim, code, lo que uses
Escribe algo de contenido y guarda el archivo.
Inicializa Git en la carpeta:
git init
Esto crea un repo local.
Verifica el estado del repo:
git status
Muestra archivos sin seguimiento, cambios, etc.
3️⃣ Agregar archivos al staging y hacer commits
Agregar todos los archivos:
git add .
Agregar un archivo específico:
git add README.md
Hacer commit (guardar cambios localmente):
git commit -m "Primer commit: agrego README"
Cada commit es un punto de control de tu proyecto.
4️⃣ Conectar el repositorio local con GitHub
Crear un repo en GitHub (puede ser público o privado).
Agregar el remoto origin:
git remote add origin https://github.com/TuUsuario/TuRepo.git
Verificar que se agregó:
git remote -v
5️⃣ Subir cambios a GitHub (push)
Primera vez:
git push -u origin main
-u establece la rama main como rama por defecto para subir cambios.
En los siguientes commits:
git add .
git commit -m "Mensaje descriptivo"
git push
6️⃣ Mantener el repositorio sincronizado
Traer cambios del remoto:
git pull origin main
Traer cambios sin fusionarlos automáticamente:
git fetch origin
git log HEAD..origin/main --oneline  # ver commits remotos que no tienes
7️⃣ Ver estado e historial
Estado de archivos:
git status
Historial de commits:
git log
git log --oneline   # versión resumida
Diferencias en archivos modificados:
git diff
8️⃣ Ramas (branches)
Crear una nueva rama:
git branch nombre_rama
Cambiar a otra rama:
git checkout nombre_rama
Subir una rama al remoto:
git push -u origin nombre_rama
Combinar ramas (merge):
git checkout main
git merge nombre_rama
9️⃣ Archivos y carpetas en repositorio
Para subir archivos individuales:
git add archivo.md
git commit -m "Agrego archivo específico"
git push
Para subir carpetas completas:
git add carpeta/
git commit -m "Agrego carpeta con contenido"
git push
10️⃣ Consejos prácticos
Mantén tus commits pequeños y descriptivos.
Usa carpetas para organizar archivos (temas/, guia/, imagenes/, etc.).
Si trabajas en un repo compartido, siempre git pull antes de hacer push.
Para repos privados, nunca compartas tu token públicamente.

💡 Resumen de flujo básico:

Crear carpeta → git init → crear archivos → git add → git commit → git remote add origin → git push
Cambios futuros: git add → git commit → git push → git pull para sincronizar
