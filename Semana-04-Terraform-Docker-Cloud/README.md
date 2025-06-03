# 📅 Semana 04 - Terraform + Proveedor Docker

## 🎯 Objetivo de la Semana
Entender los fundamentos de Terraform como herramienta de IaC (Infraestructura como Código) y cómo usar el proveedor Docker para gestionar contenedores de forma declarativa.

---

## 📘 Teoría

### 🌱 Fundamentos de Terraform

- **¿Qué es Terraform y qué problema resuelve?**
  - 🎥 [Curso Completo de Terraform | De Principiante a Avanzado](https://www.youtube.com/watch?v=Z94DYoF5ufg)
  - ✅ *Práctica:* Explica con tus palabras cómo IaC mejora la gestión de infraestructura.

- **Instalación y comandos básicos: `init`, `plan`, `apply`, `destroy`**
  - 🎥 [Curso de Terraform: Aprende infraestructura como código - Parte 1](https://www.youtube.com/watch?v=9OG9ZwvTPQY)
  - ✅ *Práctica:* Inicializa un proyecto y prueba los comandos en una carpeta vacía.

- **Estructura de un archivo `.tf`: provider, resource, variable**
  - 🎥 [Aprendiendo a automatizar con Terraform - Nerdearla 2020](https://www.youtube.com/watch?v=p3XYCneP2-Q)
  - ✅ *Práctica:* Crea un archivo `main.tf` con un proveedor cualquiera y declara un recurso.

---

## 🐳 Proveedor Docker

- **¿Qué es el proveedor Docker?**
  - 📘 [Documentación oficial del proveedor Docker](https://registry.terraform.io/providers/kreuzwerker/docker/latest/docs)
  - ✅ *Práctica:* Lista los recursos disponibles y para qué sirven (`docker_image`, `docker_container`, etc.)

- **Crear y levantar contenedores desde Terraform**
  - 🎥 [Terraform + Docker: despliegue automático - David Armendáriz](https://www.youtube.com/watch?v=FHTWRIzvGjc)
  - ✅ *Práctica:* Crea un archivo `main.tf` que levante un contenedor `nginx` en el puerto 8080.

---

## 🧪 Ejercicios

1. Instala Terraform y Docker en tu sistema.
2. Crea un archivo `main.tf` con el proveedor Docker.
3. Declara una imagen de nginx y levanta un contenedor.
4. Expón el servicio en el puerto 8080.
5. Elimina los recursos con `terraform destroy`.

---

## 🛠 Proyecto: "Infraestructura Declarativa con Docker"

**Objetivo:** Usar Terraform para levantar una infraestructura con contenedores Docker completamente definida desde código.

### Estructura esperada:
```
infra-docker/
├── main.tf
├── Dockerfile
└── index.html
```


### Requisitos del proyecto:

- Crear una red personalizada de Docker.
- Crear una imagen personalizada con un `Dockerfile`.
- Levantar un contenedor `nginx` con una página personalizada.
- Levantar un segundo contenedor `mysql`.
- Exponer el servicio web en el puerto 8080.
- Todo definido desde Terraform.

---

## 🎯 Mini-Quiz (respuestas al final)

1. ¿Qué hace `terraform init`?  
   a) Aplica los cambios  
   b) Inicializa el proyecto  
   c) Elimina los recursos

2. ¿Qué archivo contiene la configuración principal de Terraform?  
   a) `Dockerfile`  
   b) `main.tf`  
   c) `docker-compose.yml`

3. ¿Cuál es la función del proveedor Docker?  
   a) Instalar Docker  
   b) Gestionar contenedores desde Terraform  
   c) Crear scripts Bash

4. ¿Qué comando destruye los recursos?  
   a) `terraform stop`  
   b) `terraform down`  
   c) `terraform destroy`

5. ¿Terraform es una herramienta de...?  
   a) CI/CD  
   b) IaC  
   c) Virtualización

---

## 📺 Recursos Gratuitos

### Videos
- [Curso Completo de Terraform | De Principiante a Avanzado](https://www.youtube.com/watch?v=Z94DYoF5ufg)
- [Curso de Terraform: Aprende infraestructura como código - Parte 1](https://www.youtube.com/watch?v=9OG9ZwvTPQY)
- [Aprendiendo a automatizar con Terraform - Nerdearla 2020](https://www.youtube.com/watch?v=p3XYCneP2-Q)
- [Terraform + Docker: despliegue automático - David Armendáriz](https://www.youtube.com/watch?v=FHTWRIzvGjc)

### Documentación
- [Terraform Docs (oficial)](https://developer.hashicorp.com/terraform/docs)
- [Proveedor Docker (kreuzwerker)](https://registry.terraform.io/providers/kreuzwerker/docker/latest/docs)

---

## ✅ Respuestas del Mini-Quiz

1. ✅ b) Inicializa el proyecto  
2. ✅ b) `main.tf`  
3. ✅ b) Gestionar contenedores desde Terraform  
4. ✅ c) `terraform destroy`  
5. ✅ b) IaC
