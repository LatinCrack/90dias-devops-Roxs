# 📅 Semana 07 - Seguridad en Contenedores, Troubleshooting y Performance

## 🎯 Objetivo de la Semana
Comprender buenas prácticas de seguridad en entornos Docker/Kubernetes, diagnosticar errores comunes en contenedores y optimizar el rendimiento de nuestros servicios.

---

## 📘 Teoría

### 🔐 Seguridad en contenedores

- 🛡️ ¿Por qué es importante la seguridad en contenedores?
  - 🎥 [Docker Security Best Practices - TechWorld with Nana (Español Sub)](https://www.youtube.com/watch?v=kp_exzW6zdc)
  - 📘 [Docker Docs - Seguridad](https://docs.docker.com/security/)
  - ✅ *Práctica:* Analiza una imagen con `docker scan` (requiere Docker Desktop o cuenta en DockerHub).

- 🧪 Escaneo de imágenes y reducción de superficie de ataque
  - 🎥 [Trivy - Scanner de vulnerabilidades para contenedores](https://www.youtube.com/watch?v=lx5BhA4vVxE)
  - 📘 [Aqua Trivy - GitHub oficial](https://github.com/aquasecurity/trivy)
  - ✅ *Práctica:* Instala `trivy` y escanea una imagen oficial (`nginx`, `node`, etc.)

- ⚙️ Principios de imágenes seguras y buenas prácticas
  - 🎥 [Dockerfile seguro - Devtalles](https://www.youtube.com/watch?v=diBvDByvY6M)
  - ✅ *Práctica:* Crea un Dockerfile con usuario no root, sin capas innecesarias y usando `alpine`.

---

### 🛠 Troubleshooting en Docker/Kubernetes

- 🐞 Diagnóstico de contenedores y errores comunes (`docker logs`, `docker exec`, `kubectl describe`, `kubectl logs`)
  - 🎥 [Solución de problemas en Docker - Juan Villalvazo](https://www.youtube.com/watch?v=wF6rgS_GaDM)
  - 🎥 [Troubleshooting Kubernetes - Bret Fisher (sub en español)](https://www.youtube.com/watch?v=qi8bY_xwZfM)
  - ✅ *Práctica:* Simula un error de red, de permisos o de imagen inexistente y localízalo con logs.

- 🧪 Herramientas para depuración
  - 📘 [K9s - UI para clúster Kubernetes](https://k9scli.io/)
  - 🎥 [K9s - Aprende a usarlo en minutos - Devtalles](https://www.youtube.com/watch?v=zNS0V1l2zfg)
  - ✅ *Práctica:* Instala `k9s` y navega en tus pods para ver el estado en tiempo real.

---

### 🚀 Optimización de contenedores

- 🔍 Monitoreo básico con `docker stats` y `kubectl top`
  - 📘 [Docker stats - Docs](https://docs.docker.com/engine/reference/commandline/stats/)
  - 🎥 [Kubernetes Resource Metrics - The Cloud Bootcamp](https://www.youtube.com/watch?v=nkkk7IjrTRI)
  - ✅ *Práctica:* Evalúa el consumo de CPU y memoria en tus contenedores.

- 🪛 Buenas prácticas de rendimiento (multi-stage builds, imágenes mínimas, uso de cache)
  - 🎥 [Multi-stage builds explicados - La Cocina del Código](https://www.youtube.com/watch?v=lQpEOnbDkUc)
  - ✅ *Práctica:* Refactoriza un Dockerfile usando build multi-stage y compara el tamaño final.

---

## 🧪 Ejercicios

1. Instala Trivy y escanea 3 imágenes distintas (una oficial, una tuya y una de DockerHub).
2. Usa `docker stats` para ver el rendimiento en contenedores y documenta los valores.
3. Crea un Dockerfile con buenas prácticas de seguridad (usuario no root, imagen base pequeña).
4. Simula un error común (puerto ocupado, falta de permisos) y resuélvelo con `logs` y `exec`.
5. Usa `kubectl top` o `k9s` para evaluar el consumo de recursos de un pod.

---

## 🛠 Proyecto: “Contenedor Blindado”

**Objetivo:** Crear una imagen segura, optimizada y monitoreada con herramientas de troubleshooting activas.

### Requisitos:
- Dockerfile multi-stage con buenas prácticas.
- Imagen escaneada y validada con Trivy.
- Scripts de monitoreo con `docker stats` o `kubectl top`.
- Documentación del proceso de diagnóstico ante errores intencionados.

---

## 🎯 Mini-Quiz (respuestas al final)

1. ¿Qué hace Trivy?
   a) Escanea logs  
   b) Escanea vulnerabilidades en imágenes  
   c) Crea imágenes Docker  

2. ¿Cuál es el comando para ver el consumo de recursos en Docker?
   a) `docker run`  
   b) `docker ps`  
   c) `docker stats`  

3. ¿Qué opción mejora la seguridad de una imagen?
   a) Ejecutar como root  
   b) Usar imagen Alpine  
   c) Añadir más capas  

4. ¿Qué hace `kubectl logs`?
   a) Muestra recursos  
   b) Muestra registros de un pod  
   c) Borra pods  

5. ¿Qué es `multi-stage build`?
   a) Técnica para construir imágenes con múltiples etapas  
   b) Herramienta de monitoreo  
   c) Clúster de staging  

---

## 📺 Recursos Gratuitos

### Videos
- [Docker Security Best Practices - TechWorld with Nana](https://www.youtube.com/watch?v=kp_exzW6zdc)
- [Trivy - Escaneo de vulnerabilidades](https://www.youtube.com/watch?v=lx5BhA4vVxE)
- [Troubleshooting Kubernetes - Bret Fisher](https://www.youtube.com/watch?v=qi8bY_xwZfM)
- [Dockerfile seguro - Devtalles](https://www.youtube.com/watch?v=diBvDByvY6M)
- [Multi-stage builds - La Cocina del Código](https://www.youtube.com/watch?v=lQpEOnbDkUc)
- [K9s explicado en minutos - Devtalles](https://www.youtube.com/watch?v=zNS0V1l2zfg)

### Documentación
- https://docs.docker.com/security/
- https://github.com/aquasecurity/trivy
- https://docs.docker.com/engine/reference/commandline/stats/
- https://k9scli.io/

---

## ✅ Respuestas del Mini-Quiz

1. ✅ b) Escanea vulnerabilidades en imágenes  
2. ✅ c) `docker stats`  
3. ✅ b) Usar imagen Alpine  
4. ✅ b) Muestra registros de un pod  
5. ✅ a) Técnica para construir imágenes con múltiples etapas
