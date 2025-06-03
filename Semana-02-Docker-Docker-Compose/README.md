# 📅 Semana 02 - Docker y Docker Compose

## 🎯 Objetivo de la Semana
Comprender el funcionamiento de contenedores usando Docker, construir imágenes personalizadas y levantar múltiples servicios usando Docker Compose.

---

## 📘 Teoría

### 🐳 Fundamentos de Docker

- **¿Qué es un contenedor? ¿Cómo se diferencia de una máquina virtual?**
  - 🎥 [Docker explicado en 7 minutos - Fireship](https://www.youtube.com/watch?v=Gjnup-PuquQ)
  - ✅ *Práctica:* Haz un esquema comparando contenedores vs máquinas virtuales.

- **Arquitectura de Docker (cliente, demonio, imágenes, contenedores, registries)**
  - 🎥 [Aprende Docker ahora! curso completo gratis desde cero! - HolaMundo](https://www.youtube.com/watch?v=4Dko5W96WHg)
  - ✅ *Práctica:* Dibuja el flujo desde que creas una imagen hasta que levantas un contenedor.

- **Comandos básicos: `docker run`, `ps`, `images`, `build`, `exec`, `stop`, `rm`, `rmi`**
  - 🎥 [Docker, Curso Práctico para principiantes (desde Linux) - Fazt](https://www.youtube.com/watch?v=NVvZNmfqg6M)
  - ✅ *Práctica:* Crea un contenedor de `nginx`, accede, cambia el contenido de `/usr/share/nginx/html` y expón el servicio.

- **Crear una imagen desde un Dockerfile**
  - 🎥 [¿Qué es DOCKERFILE? ¿Cómo trabajar con él? - La Cocina del Código](https://www.youtube.com/watch?v=0f2pHstRjow)
  - ✅ *Práctica:* Crea una imagen que sirva un sitio web estático con nginx personalizado.

### 🛠 Docker Compose

- **¿Qué es y para qué sirve Docker Compose?**
  - 🎥 [Docker Compose en 100 segundos - Webtips](https://www.youtube.com/watch?v=Gjnup-PuquQ)
  - ✅ *Práctica:* Resume con tus palabras cuándo usarías Docker Compose.

- **Archivo `docker-compose.yml`: estructura básica**
- **Levantar múltiples servicios (`docker-compose up`, `down`)**
  - 🎥 [Curso Docker desde cero - HolaMundo](https://www.youtube.com/watch?v=4Dko5W96WHg)
  - ✅ *Práctica:* Crea un `docker-compose.yml` que levante `nginx` + `mysql` y verifica que ambos funcionen.

---

## 🧪 Ejercicios

1. Instala Docker y Docker Compose.
2. Ejecuta una imagen oficial de `nginx` en un contenedor.
3. Personaliza un `index.html` en tu contenedor nginx.
4. Crea un Dockerfile para servir tu propia web estática.
5. Usa Docker Compose para levantar `nginx` y `mysql` en red.
6. Visualiza los logs y recursos consumidos por tus contenedores.

---

## 🛠 Proyecto: "Puerto DevOps"

**Objetivo:** Crear un entorno con dos servicios usando Docker Compose: un servidor web (`nginx`) y una base de datos (`mysql`).

### Estructura esperada:
```
puerto-devops/
├── docker-compose.yml
├── nginx/
│ └── index.html
└── db/
└── init.sql
```


### Requisitos del proyecto:
- Servicio web que responda en el puerto 8080 con una página personalizada.
- Servicio de base de datos MySQL con usuario, contraseña y base creada desde `init.sql`.
- Ambos servicios deben conectarse por red interna y logs deben ser visibles.

---

## 🎯 Mini-Quiz (respuestas al final del archivo)

1. ¿Qué comando permite ver los contenedores en ejecución?  
   a) `docker exec`  
   b) `docker ps`  
   c) `docker start`

2. ¿Qué archivo se utiliza para definir múltiples servicios en Docker Compose?  
   a) `Dockerfile`  
   b) `compose.yaml`  
   c) `docker-compose.yml`

3. ¿Cuál es la diferencia principal entre `docker build` y `docker run`?  
   a) `build` descarga imágenes, `run` las borra  
   b) `build` crea imágenes, `run` ejecuta contenedores  
   c) No hay diferencia

4. ¿Qué hace el comando `docker-compose down`?  
   a) Inicia los servicios  
   b) Destruye los contenedores y redes creadas  
   c) Reinicia los servicios

5. ¿Qué puerto se expone por defecto en una imagen `nginx`?  
   a) 22  
   b) 80  
   c) 443

---

## 📺 Recursos Gratuitos

### Videos
- [Docker explicado en 7 minutos - Fireship](https://www.youtube.com/watch?v=Gjnup-PuquQ)
- [Aprende Docker ahora! curso completo gratis desde cero! - HolaMundo](https://www.youtube.com/watch?v=4Dko5W96WHg)
- [Docker, Curso Práctico para principiantes - Fazt](https://www.youtube.com/watch?v=NVvZNmfqg6M)
- [¿Qué es DOCKERFILE? - La Cocina del Código](https://www.youtube.com/watch?v=0f2pHstRjow)

### Documentación
- https://docs.docker.com/
- https://docs.docker.com/compose/
- https://hub.docker.com/

---

## ✅ Respuestas del Mini-Quiz
1. ✅ b) `docker ps`  
2. ✅ c) `docker-compose.yml`  
3. ✅ b) `build` crea imágenes, `run` ejecuta contenedores  
4. ✅ b) Destruye los contenedores y redes creadas  
5. ✅ b) 80
