# 📅 Semana 09 - LocalStack y Simulación de Nube AWS

## 🎯 Objetivo de la Semana
Aprender a simular servicios de AWS localmente con LocalStack, entender sus ventajas y usos, y practicar automatización de infraestructura en un entorno aislado y gratuito.

---

## 📘 Teoría

### ☁️ ¿Qué es LocalStack?

- 🎥 [¿Qué es LocalStack y para qué sirve? - DevTalles](https://www.youtube.com/watch?v=AZpBgvhxKTI)
- 📘 [Documentación Oficial de LocalStack](https://docs.localstack.cloud/)
- ✅ *Práctica:* Explica con tus palabras cuándo y por qué usarías LocalStack.

---

### 🧱 Servicios que se pueden simular

- 🎥 [Simula AWS Localmente con LocalStack - La Cocina del Código](https://www.youtube.com/watch?v=a3-OJ2rTtVQ)
- 📘 [Lista de servicios compatibles](https://docs.localstack.cloud/user-guide/aws/feature-coverage/)
- ✅ *Práctica:* Enumera al menos 5 servicios de AWS que puedes usar con LocalStack (ej: S3, Lambda, DynamoDB).

---

### ⚙️ Instalación y ejecución de LocalStack

- 🎥 [Cómo usar LocalStack paso a paso - Midudev](https://www.youtube.com/watch?v=7a8CKSO3jvU)
- 📘 [Guía rápida oficial](https://docs.localstack.cloud/get-started/)
- ✅ *Práctica:* Instala LocalStack con Docker y valida que puedas ejecutar `localstack status`.

---

### 🔧 Integración con AWS CLI y Terraform

- 🎥 [Terraform + LocalStack demo - DevOps by Example](https://www.youtube.com/watch?v=wulBSWnWTHE)
- 📘 [Configuración con AWS CLI](https://docs.localstack.cloud/user-guide/aws/aws-cli/)
- ✅ *Práctica:* Usa AWS CLI con LocalStack para crear un bucket en S3 y subir un archivo.

---

## 🧪 Ejercicios

1. Instala LocalStack con Docker.
2. Configura AWS CLI con endpoint local.
3. Crea un bucket S3 en LocalStack y sube un archivo.
4. Simula una función Lambda que procese datos desde S3.
5. Usa Terraform para automatizar la creación de recursos en LocalStack.

---

## 🛠 Proyecto: “MiniNube DevOps”

**Objetivo:** Simular un pequeño flujo en la nube con S3 + Lambda + Terraform usando LocalStack.

### Requisitos del Proyecto:
- Crear un bucket en S3.
- Subir un archivo desde tu máquina local.
- Ejecutar una función Lambda al detectar un nuevo archivo.
- Definir toda la infraestructura con Terraform.
- Documentar todo el flujo en un `README.md`.

---

## 🎯 Mini-Quiz (respuestas al final del archivo)

1. ¿Qué es LocalStack?
   a) Un editor de texto  
   b) Una herramienta para simular servicios de AWS localmente  
   c) Un cliente de base de datos  

2. ¿Qué comando permite comprobar el estado de LocalStack?
   a) `localstack info`  
   b) `localstack status`  
   c) `aws local status`  

3. ¿Cuál de estos servicios puedes simular con LocalStack?
   a) GitHub Actions  
   b) Docker Compose  
   c) AWS S3  

4. ¿Cuál es el principal beneficio de usar LocalStack?
   a) Pagar menos en AWS  
   b) Simular infraestructura sin conexión ni costos  
   c) Conectarse más rápido a Internet  

5. ¿Cómo puedes usar AWS CLI con LocalStack?
   a) Con configuración por endpoint local  
   b) No se puede  
   c) Solo con GUI

---

## 📺 Recursos Gratuitos

### Videos
- [¿Qué es LocalStack? - DevTalles](https://www.youtube.com/watch?v=AZpBgvhxKTI)
- [Simula AWS Localmente - La Cocina del Código](https://www.youtube.com/watch?v=a3-OJ2rTtVQ)
- [Usar LocalStack paso a paso - Midudev](https://www.youtube.com/watch?v=7a8CKSO3jvU)
- [Terraform + LocalStack demo - DevOps by Example](https://www.youtube.com/watch?v=wulBSWnWTHE)

### Documentación
- https://docs.localstack.cloud/
- https://docs.localstack.cloud/user-guide/aws/aws-cli/
- https://docs.localstack.cloud/user-guide/aws/feature-coverage/
- https://docs.localstack.cloud/get-started/

---

## ✅ Respuestas del Mini-Quiz

1. ✅ b) Una herramienta para simular servicios de AWS localmente  
2. ✅ b) `localstack status`  
3. ✅ c) AWS S3  
4. ✅ b) Simular infraestructura sin conexión ni costos  
5. ✅ a) Con configuración por endpoint local
