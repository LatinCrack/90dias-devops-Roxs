# 📅 Semana 06 - Despliegue con CI/CD a Kubernetes

## 🎯 Objetivo de la Semana
Automatizar el flujo de integración continua y despliegue continuo (CI/CD) hacia un clúster de Kubernetes utilizando GitHub Actions.

---

## 📘 Teoría

### 🔄 ¿Qué es CI/CD en DevOps?

- 🎥 [¿Qué es CI/CD y cómo funciona? - Fazt](https://www.youtube.com/watch?v=Qr4QMBUPxWo)
- 📘 [Guía CI/CD de GitHub](https://docs.github.com/es/actions/guides/about-continuous-integration)
- ✅ *Práctica:* Resume con tus palabras qué pasos debe tener un pipeline de CI/CD.

---

### 🤖 GitHub Actions para Kubernetes

- 🧠 ¿Cómo integrar GitHub Actions con Kubernetes?
  - 🎥 [GitHub Actions + Kubernetes con Helm - Techworld with Nana](https://www.youtube.com/watch?v=48VQJbZRgZQ)
  - 📘 [GitHub Actions Marketplace - kubectl](https://github.com/marketplace/actions/kubectl-tool-installer)
  - ✅ *Práctica:* Analiza un workflow YAML que construya una imagen y la despliegue con `kubectl`.

---

### 📦 Construcción y Despliegue de Imágenes

- 🔨 Construir y subir imágenes a DockerHub/GitHub Container Registry
  - 🎥 [CI/CD con GitHub Actions y DockerHub - José Dimas Luján](https://www.youtube.com/watch?v=FfvfCtwl-KM)
  - 📘 [GitHub Actions Docs - Docker](https://docs.github.com/en/actions/publishing-packages/publishing-docker-images)
  - ✅ *Práctica:* Modifica un workflow que haga `docker build`, `docker tag` y `docker push`.

---

### 🚀 Despliegue automático en Kubernetes

- 📥 Crear archivo de despliegue (`deployment.yaml`, `service.yaml`)
  - 🎥 [Kubernetes Deployment explicado - Código Mentable](https://www.youtube.com/watch?v=9vZlxsiCkXU)
  - ✅ *Práctica:* Crea un manifiesto Kubernetes para desplegar una imagen tuya.

- 🤖 Automatizar despliegue con `kubectl apply`
  - 🎥 [CI/CD Pipeline completo hacia Kubernetes - The Cloud Bootcamp](https://www.youtube.com/watch?v=4OBu5O6wENg)
  - ✅ *Práctica:* Usa `kubectl` en un pipeline para aplicar tus archivos `.yaml`.

---

## 🧪 Ejercicios

1. Crea un workflow que construya tu imagen y la suba a DockerHub.
2. Genera tus archivos `deployment.yaml` y `service.yaml`.
3. Usa GitHub Actions para aplicar los manifiestos en un clúster de Minikube/Kind.
4. Simula un cambio en la aplicación y verifica si se despliega automáticamente.

---

## 🛠 Proyecto: “Kube Delivery”

**Objetivo:** Implementar CI/CD que despliegue una aplicación de forma automática en Kubernetes usando GitHub Actions.

### Requisitos:
- Repositorio en GitHub con Dockerfile, workflow y manifiestos.
- Acción que haga `build`, `push` y `kubectl apply`.
- Acceso al clúster desde GitHub (token, config o kubeconfig secreta).
- Logs visibles del pipeline.

---

## 🎯 Mini-Quiz (respuestas al final)

1. ¿Qué hace `docker push`?
   a) Ejecuta una imagen  
   b) Construye una imagen  
   c) Sube una imagen a un registry  

2. ¿Qué archivo define las acciones de CI/CD en GitHub?
   a) `Dockerfile`  
   b) `.github/workflows/*.yml`  
   c) `deployment.yaml`  

3. ¿Qué comando se usa para aplicar cambios en Kubernetes?
   a) `kubectl deploy`  
   b) `kubectl apply -f archivo.yaml`  
   c) `kubectl start`  

4. ¿Dónde se almacenan los secretos en GitHub Actions?
   a) `.secrets`  
   b) GitHub Settings → Secrets  
   c) Dentro del workflow  

5. ¿Qué hace un archivo `deployment.yaml`?
   a) Ejecuta pods aleatorios  
   b) Define cómo se despliega una aplicación en Kubernetes  
   c) Instala Kubernetes  

---

## 📺 Recursos Gratuitos

### Videos
- [¿Qué es CI/CD? - Fazt](https://www.youtube.com/watch?v=Qr4QMBUPxWo)
- [CI/CD con GitHub Actions y DockerHub](https://www.youtube.com/watch?v=FfvfCtwl-KM)
- [GitHub Actions + Kubernetes con Helm](https://www.youtube.com/watch?v=48VQJbZRgZQ)
- [CI/CD Pipeline hacia Kubernetes - The Cloud Bootcamp](https://www.youtube.com/watch?v=4OBu5O6wENg)
- [Deployment explicado en Kubernetes](https://www.youtube.com/watch?v=9vZlxsiCkXU)

### Documentación
- https://docs.github.com/es/actions/guides/about-continuous-integration  
- https://docs.github.com/en/actions/publishing-packages/publishing-docker-images  
- https://kubernetes.io/docs/concepts/workloads/controllers/deployment/  
- https://github.com/marketplace/actions/kubectl-tool-installer  

---

## ✅ Respuestas del Mini-Quiz

1. ✅ c) Sube una imagen a un registry  
2. ✅ b) `.github/workflows/*.yml`  
3. ✅ b) `kubectl apply -f archivo.yaml`  
4. ✅ b) GitHub Settings → Secrets  
5. ✅ b) Define cómo se despliega una aplicación en Kubernetes
