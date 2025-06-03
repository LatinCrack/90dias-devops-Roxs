# 📅 Semana 03 - GitHub Actions y CI/CD

## 🎯 Objetivo de la Semana
Aprender a automatizar procesos de integración continua y despliegue continuo (CI/CD) usando GitHub Actions para mejorar la productividad y calidad del software.

---

## 📘 Teoría

### 🔄 ¿Qué es CI/CD?

- **Integración Continua (CI):** Automatización del proceso de pruebas y construcción del código cada vez que se hacen cambios.
- **Despliegue Continuo (CD):** Automatización para desplegar el software a ambientes de prueba o producción automáticamente.

### 🛠 GitHub Actions

- **¿Qué es GitHub Actions?**
  - Plataforma de automatización integrada en GitHub para crear workflows (flujos de trabajo) que ejecutan tareas en eventos definidos.
  - 🎥 [GitHub Actions Tutorial para Principiantes - Fazt](https://www.youtube.com/watch?v=R8_veQiYBjI)

- **Componentes principales**
  - Workflow: archivo YAML que define el flujo.
  - Jobs: tareas que se ejecutan.
  - Steps: pasos dentro de un job.
  - Runners: servidores que ejecutan los jobs.

- **Eventos comunes para disparar workflows**
  - Push, Pull Request, Releases, Programación (cron), etc.

- **Sintaxis básica de un workflow**
  - 🎥 [GitHub Actions: Configuración básica - FreeCodeCamp](https://www.youtube.com/watch?v=0yWAtQ6wYNM)

---

## 🧪 Ejercicios

1. Crea un repositorio en GitHub y conecta tu código local.
2. Configura un workflow básico que se ejecute en cada push y haga un build simple.
3. Agrega un job que corra pruebas unitarias.
4. Configura notificaciones por email o Slack (opcional).
5. Automatiza el despliegue a GitHub Pages o a un servidor remoto (si aplica).

---

## 🛠 Proyecto: Pipeline Básico CI/CD

**Objetivo:** Crear un pipeline en GitHub Actions que construya, pruebe y despliegue automáticamente una aplicación web simple.

### Pasos sugeridos:

- Crear un repositorio con una aplicación básica (por ejemplo, React, Node.js o una página estática).
- Añadir un archivo `.github/workflows/ci.yml` con las siguientes etapas:
  - Checkout del código.
  - Instalación de dependencias.
  - Ejecución de tests.
  - Despliegue a GitHub Pages (si aplica).
  
### Ejemplo básico workflow:
```yaml
name: CI

on:
  push:
    branches: [ main ]

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v3
    - name: Setup Node.js
      uses: actions/setup-node@v3
      with:
        node-version: '16'
    - name: Install dependencies
      run: npm install
    - name: Run tests
      run: npm test
    - name: Deploy to GitHub Pages
      if: github.ref == 'refs/heads/main'
      uses: peaceiris/actions-gh-pages@v3
      with:
        github_token: ${{ secrets.GITHUB_TOKEN }}
        publish_dir: ./build
```

## 🎯 Mini-Quiz (respuestas al final del archivo)

1. ¿Qué archivo define un workflow en GitHub Actions?
   a) .gitignore
   b) .github/workflows/*.yml
   c) Dockerfile

2. ¿Cuál es el evento que comúnmente dispara un workflow?
   a) commit
   b) push
   c) merge  

3. Qué hace un job en GitHub Actions?
   a) Ejecuta un conjunto de pasos 
   b) Despliega la aplicación
   c) Modifica el repositorio  

4. ¿Qué se necesita para desplegar a GitHub Pages usando Actions?
   a) Token de acceso
   b) Archivo Dockerfile
   c) Script bash  

5. ¿Cuál es la plataforma que ejecuta los workflows de GitHub Actions?
   a) Runners
   b) Pods
   c) Clusters  

---
## 📺 Recursos Gratuitos

### Videos
- [GitHub Actions Tutorial para Principiantes - Fazt](https://www.youtube.com/watch?v=R8_veQiYBjI)
- [GitHub Actions: Configuración básica - FreeCodeCamp](https://www.youtube.com/watch?v=0yWAtQ6wYNM)
- [CI/CD con GitHub Actions - Código Facilito](https://www.youtube.com/watch?v=qX3DLD9nF0A)


### Documentación
- https://docs.github.com/en/actions (https://docs.github.com/en/actions)
- https://docs.github.com/en/actions/using-workflows (https://docs.github.com/en/actions/using-workflows)
- https://docs.github.com/en/actions/deployment (https://docs.github.com/en/actions/deployment)

---

## ✅ Respuestas del Mini-Quiz
1. ✅ b) .github/workflows/*.yml 
2. ✅ b) push  
3. ✅ a) Ejecuta un conjunto de pasos  
4. ✅ a) Token de acceso  
5. ✅ a) Runners

