# 📘 Guía básica de Git y GitHub

Aprende a usar Git desde cero con ejemplos simples, comandos esenciales y soluciones a errores comunes.

---

## 🚀 Subir tu primer proyecto a GitHub (paso a paso)

### 1️⃣ Inicializa el repositorio

```
git init
```

### 2️⃣ Agrega los archivos

```
git add .
```

### 3️⃣ Guarda los cambios

```
git commit -m "Primer commit"
```

### 4️⃣ Conecta con GitHub

```
git remote add origin URL_DE_TU_REPOSITORIO
```

### 5️⃣ Sube tu proyecto

```
git push -u origin main
```

---

## 📂 Comandos básicos

### 🔍 Ver estado del proyecto

```
git status
```

Muestra los archivos modificados y los que están listos para guardar.

---

### ➕ Agregar archivos

```
git add .
git add archivo.txt
```

Prepara los archivos antes de hacer commit.

---

### 💾 Guardar cambios

```
git commit -m "Mensaje"
```

Guarda una versión del proyecto.

---

### ☁️ Subir cambios

```
git push origin main
```

Sube tus cambios a GitHub.

---

### 📥 Descargar repositorio

```
git clone URL
```

Copia un repositorio a tu computadora.

---

### 🔄 Actualizar proyecto

```
git pull origin main
```

Descarga cambios nuevos del repositorio.

---

## 🌿 Manejo de ramas

### Crear una rama

```
git branch nombre-rama
```

### Cambiar de rama

```
git checkout nombre-rama
```

### Unir ramas

```
git merge nombre-rama
```

---

## ❌ Errores comunes y soluciones

### error: failed to push

```
git pull origin main --rebase
```

Solución: primero debes actualizar tu repositorio antes de subir cambios.

---

### error: repository not found

Verifica:

* URL correcta del repositorio
* Que tienes acceso

---

### cambios no guardados al cambiar de rama

```
git stash
```

Guarda cambios temporalmente.

---

## 💡 Tips útiles

### Ver historial resumido

```
git log --oneline
```

### Deshacer cambios en un archivo

```
git restore archivo.txt
```

### Ver ramas

```
git branch
```

---

## 🧠 Conceptos clave

* **Git**: sistema de control de versiones
* **GitHub**: plataforma para almacenar y compartir código
* **Commit**: guardado de cambios
* **Push**: subir cambios
* **Pull**: descargar cambios

---

## 🎯 Objetivo

Esta guía está hecha para:

* Principiantes en Git
* Personas que quieren un resumen rápido
* Tener comandos esenciales en un solo lugar

---

## ⭐ Si te sirve

Dale una estrella al repositorio y compártelo 🙌
