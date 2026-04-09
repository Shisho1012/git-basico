# 🚀 Git y GitHub desde cero (sin romper nada)

Aprende Git de forma simple, práctica y sin complicarte 😄
Esta guía está pensada para **personas que empiezan y no saben por dónde empezar**.

---

## ⚡ Lo mínimo que necesitas saber

👉 En la vida real, casi siempre usarás esto:

```bash
git add .
git commit -m "mensaje"
git push
git pull
```

🧠 Flujo mental:
**cambiar → guardar → subir**

---

## 🚀 Tu primer proyecto en GitHub (PASO A PASO)

Sigue esto exactamente 👇

```bash
# Crear carpeta del proyecto
mkdir mi-proyecto
cd mi-proyecto

# Inicializar repositorio
git init

# Crear README vacío
touch README.md

# Primer commit
git add README.md
git commit -m "Agregando README inicial"

# Agregar otros archivos y commit
git add .
git commit -m "Primer commit con archivos"

# Conectar con GitHub
git remote add origin URL_DE_TU_REPO

# Subir a GitHub
git push -u origin main
```

✅ Si esto funciona, ya sabes usar Git básico.

---

## 🔁 Flujo real de trabajo

Cada vez que hagas cambios:

```bash
git add .
git commit -m "cambios"
git push
```

Y antes de trabajar:

```bash
git pull
```

---

## 📂 Comandos importantes (explicados fácil)

### 🔍 Ver estado

```bash
git status
```

👉 Te dice qué cambió

---

### ➕ Agregar cambios

```bash
git add .
```

👉 Prepara archivos para guardar

---

### 💾 Guardar cambios

```bash
git commit -m "mensaje"
```

👉 Guarda una versión

---

### ☁️ Subir cambios

```bash
git push
```

👉 Lo manda a GitHub

---

### 📥 Descargar repo

```bash
git clone URL
```

---

### 🔄 Actualizar proyecto

```bash
git pull
```

---

## 🌿 Ramas (sin complicarte)

```bash
git branch nueva-rama
git checkout nueva-rama
git merge nueva-rama
```

💡 Sirven para no romper el proyecto principal.

---

## ❌ Errores comunes (esto te salvará)

### 🔴 No te deja hacer push

```bash
git pull --rebase
```

👉 Pasa cuando el repo cambió antes que tú.

---

### 🔴 Cambié de rama y perdí cosas

```bash
git stash
```

👉 Guarda cambios temporalmente.

---

### 🔴 Me equivoqué en un archivo

```bash
git restore archivo
```

---

## 💡 Tips que casi nadie te dice

```bash
git log --oneline     # ver historial simple
git branch            # ver ramas
git stash             # guardar cambios temporales
```

---

## 🧠 Cómo pensar Git (importante)

No memorices comandos. Piensa así:

* **add** → preparar
* **commit** → guardar
* **push** → subir
* **pull** → actualizar

---

## 🎯 ¿Para quién es esto?

* Si estás empezando en programación
* Si Git te confunde
* Si quieres algo rápido y claro

---

## ⭐ Si te ayudó

Dale estrella al repo ⭐
y compártelo con alguien que lo necesite 🙌
