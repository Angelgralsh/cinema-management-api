# 🚀 Guía para subir a GitHub

## ✅ Pasos completados:

1. ✅ Repositorio Git inicializado
2. ✅ Archivos agregados al staging
3. ✅ Primer commit creado

---

## 📝 Próximos pasos:

### 1. Crear el repositorio en GitHub

1. Ve a [GitHub](https://github.com)
2. Haz clic en el botón **"New"** o el ícono **+** → **"New repository"**
3. Completa los datos:
   - **Repository name**: `cinema-management-api` (o el nombre que prefieras)
   - **Description**: `Sistema de gestión de cine con Node.js, Express y TypeScript usando Repository Pattern`
   - **Visibility**: Elige **Public** o **Private**
   - ⚠️ **NO** marques "Initialize this repository with a README" (ya tienes uno)
4. Haz clic en **"Create repository"**

---

### 2. Conectar tu repositorio local con GitHub

Después de crear el repositorio, GitHub te mostrará comandos. Usa estos (reemplaza `TU-USUARIO` con tu usuario de GitHub):

#### Opción A: Si tu rama principal se llama "master"
```powershell
cd C:\cinema-management
git remote add origin https://github.com/TU-USUARIO/cinema-management-api.git
git branch -M main
git push -u origin main
```

#### Opción B: Si prefieres usar SSH
```powershell
cd C:\cinema-management
git remote add origin git@github.com:TU-USUARIO/cinema-management-api.git
git branch -M main
git push -u origin main
```

---

### 3. Comandos explicados:

- `git remote add origin [URL]`: Conecta tu repositorio local con GitHub
- `git branch -M main`: Renombra la rama de "master" a "main" (estándar actual)
- `git push -u origin main`: Sube tu código a GitHub

---

## 🔐 Autenticación

Si es la primera vez que usas Git con GitHub, necesitarás autenticarte:

### Opción 1: HTTPS (Recomendado)
- GitHub te pedirá usuario y contraseña
- **Importante**: Ya no se acepta contraseña normal, necesitas un **Personal Access Token**
- Crea uno en: https://github.com/settings/tokens
- Permisos necesarios: `repo` (acceso completo)

### Opción 2: SSH
- Genera una clave SSH: `ssh-keygen -t ed25519 -C "tu-email@ejemplo.com"`
- Agrega la clave a GitHub: https://github.com/settings/keys

---

## 📋 Comandos rápidos para copiar

Una vez que tengas la URL de tu repositorio en GitHub:

```powershell
# Navegar al proyecto
cd C:\cinema-management

# Agregar el repositorio remoto (reemplaza la URL)
git remote add origin https://github.com/TU-USUARIO/cinema-management-api.git

# Renombrar rama a main
git branch -M main

# Subir el código
git push -u origin main
```

---

## ✨ Después de subir

Tu proyecto estará en GitHub y podrás:
- Compartir el enlace con otros
- Colaborar con tu equipo
- Usar GitHub Actions para CI/CD
- Documentar tu proyecto con el README

---

## 🆘 Solución de problemas comunes

### Error: "remote origin already exists"
```powershell
git remote remove origin
git remote add origin https://github.com/TU-USUARIO/cinema-management-api.git
```

### Error: "Authentication failed"
- Verifica tu token de acceso personal
- O configura SSH correctamente

### Ver el estado actual
```powershell
git status
git remote -v
```

---

## 📞 ¿Necesitas ayuda?

Una vez que crees el repositorio en GitHub, dime la URL y te ayudaré con los comandos específicos.
