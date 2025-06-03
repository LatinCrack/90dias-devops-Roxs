# 📅 Semana 05 - Kubernetes local con Minikube/Kind

## 🎯 Objetivo de la Semana
Comprender los fundamentos de Kubernetes y levantar un clúster local usando Minikube o Kind. Desplegar pods, servicios y realizar pruebas básicas.

---

## 📘 Teoría

### 📦 ¿Qué es Kubernetes y por qué es esencial?

- 🎥 [KUBERNETES PARA PRINCIPIANTES (Explicado Fácil, desde Cero)](https://www.youtube.com/watch?v=DzuU1KLQ240)
- 📘 [¿Qué es Kubernetes? - Documentación Oficial](https://kubernetes.io/es/docs/concepts/overview/what-is-kubernetes/)
- ✅ *Práctica:* Resume qué resuelve Kubernetes en comparación con Docker Compose.

---

### 🧰 Instalación de Minikube o Kind

- 🛠 [Guía oficial de Minikube](https://minikube.sigs.k8s.io/docs/start/)
- 🎥 [Instalar Minikube paso a paso - Carlos Azaustre](https://www.youtube.com/watch?v=YFl2mCHdv24)
- 🛠 [Guía oficial de Kind](https://kind.sigs.k8s.io/docs/user/quick-start/)
- 🎥 [How to run local multi-node Kubernetes clusters using kind](https://www.youtube.com/watch?v=C0v5gJSWuSo)
- ✅ *Práctica:* Elige entre Minikube o Kind e instala en tu sistema operativo.

---

### 📄 Recursos básicos de Kubernetes

- **Pods, Services, Deployments, Namespaces**
  - 🎥 [Kubernetes: Fundamentos y conceptos clave - OpenWebinars](https://openwebinars.net/blog/kubernetes-fundamentos-y-conceptos-clave/)
  - 📘 [Documentación oficial de Kubernetes](https://kubernetes.io/docs/concepts/)
  - ✅ *Práctica:* Crea un archivo `pod.yaml` con nginx y levántalo con `kubectl apply -f`.

---

## 🧪 Ejercicios

1. Instala Minikube o Kind según tu sistema.
2. Verifica el clúster con `kubectl cluster-info`.
3. Crea y despliega un pod básico con nginx.
4. Expón el pod con un servicio de tipo `NodePort`.
5. Despliega un segundo pod con busybox y hazle ping al otro.

---

## 🛠 Proyecto: "Mi primer clúster Kubernetes"

**Objetivo:** Simular una pequeña infraestructura en Kubernetes localmente.

### Requisitos del proyecto:

- Crear un `Deployment` con nginx que levante 3 réplicas.
- Crear un `Service` de tipo `ClusterIP` para balancear entre las réplicas.
- Crear un `Pod` adicional con busybox para hacer pruebas de red.
- Probar escalado con `kubectl scale`.

### Estructura esperada:
```
mi-cluster-k8s/
├── deployment.yaml
├── service.yaml
└── test-pod.yaml
```

---

## 🎯 Mini-Quiz (respuestas al final)

1. ¿Qué es un Pod en Kubernetes?  
   a) Un contenedor  
   b) Un grupo de uno o más contenedores  
   c) Una red virtual

2. ¿Qué herramienta permite crear clústeres de Kubernetes locales con Docker?  
   a) Minikube  
   b) Kind  
   c) Ambas

3. ¿Cuál es el objetivo de un Service en Kubernetes?  
   a) Eliminar pods  
   b) Exponer pods  
   c) Crear clústeres

4. ¿Qué comando despliega un archivo yaml?  
   a) `kubectl start -f`  
   b) `kubectl apply -f`  
   c) `kubectl deploy -y`

5. ¿Cuál comando permite ver los pods en ejecución?  
   a) `kubectl services`  
   b) `kubectl get deployments`  
   c) `kubectl get pods`

---

## 📺 Recursos Gratuitos

### Videos
- [KUBERNETES PARA PRINCIPIANTES (Explicado Fácil, desde Cero)](https://www.youtube.com/watch?v=DzuU1KLQ240)
- [Instalar Minikube paso a paso - Carlos Azaustre](https://www.youtube.com/watch?v=YFl2mCHdv24)
- [How to run local multi-node Kubernetes clusters using kind](https://www.youtube.com/watch?v=C0v5gJSWuSo)

### Documentación
- [Documentación oficial de Kubernetes](https://kubernetes.io/docs/)
- [Guía oficial de Minikube](https://minikube.sigs.k8s.io/docs/)
- [Guía oficial de Kind](https://kind.sigs.k8s.io/docs/)

---

## ✅ Respuestas del Mini-Quiz

1. ✅ b) Un grupo de uno o más contenedores  
2. ✅ c) Ambas  
3. ✅ b) Exponer pods  
4. ✅ b) `kubectl apply -f`  
5. ✅ c) `kubectl get pods`

