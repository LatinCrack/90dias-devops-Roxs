# 📅 Semana 08 - Observabilidad y Monitoreo

## 🎯 Objetivo de la Semana
Entender los conceptos clave de observabilidad: métricas, logs y trazas, e implementar soluciones como Prometheus, Grafana y Loki para monitorear aplicaciones en Kubernetes.

---

## 📘 Teoría

### 📊 ¿Qué es la observabilidad?

- 🎥 [¿Qué es la observabilidad? - DevTalles](https://www.youtube.com/watch?v=dnS3sSQ-LK8)
- 📘 [Introducción oficial a la Observabilidad - CNCF](https://www.cncf.io/blog/2020/12/10/observability-what-it-is-and-why-it-matters/)
- ✅ *Práctica:* Resume con tus palabras la diferencia entre métricas, logs y trazas.

---

### 📈 Prometheus - Métricas

- 🎥 [¿Qué es Prometheus y cómo funciona? - DevTalles](https://www.youtube.com/watch?v=nP7pF8eyGvY)
- 📘 [Prometheus Docs - Overview](https://prometheus.io/docs/introduction/overview/)
- ✅ *Práctica:* Levanta Prometheus con Helm o docker-compose y visualiza métricas de un contenedor.

---

### 📉 Grafana - Dashboards

- 🎥 [Monitorización con Grafana + Prometheus - Midudev](https://www.youtube.com/watch?v=9iUeK0sx-PU)
- 📘 [Grafana Docs - Getting Started](https://grafana.com/docs/grafana/latest/getting-started/getting-started-prometheus/)
- ✅ *Práctica:* Conecta Prometheus a Grafana y crea un dashboard personalizado.

---

### 📜 Loki - Logs centralizados

- 🎥 [¿Qué es Loki y cómo funciona? - DevMentor](https://www.youtube.com/watch?v=CCmFgIPjeXY)
- 📘 [Grafana Loki Docs](https://grafana.com/docs/loki/latest/)
- ✅ *Práctica:* Despliega Loki y envía logs desde un contenedor con promtail.

---

## 🧪 Ejercicios

1. Instala Prometheus y Grafana con Helm o docker-compose.
2. Despliega un contenedor que exponga métricas (`nginx` o una app con `/metrics`).
3. Visualiza las métricas en un dashboard de Grafana.
4. Agrega Loki y visualiza los logs desde Promtail.
5. Simula una carga para ver cómo responde el sistema.

---

## 🛠 Proyecto: “DevOps Monitor Center”

**Objetivo:** Construir un stack de monitoreo completo con métricas y logs usando Prometheus, Grafana y Loki.

### Requisitos:
- Contenedor de `nginx` monitoreado con Prometheus.
- Logs de nginx recolectados por Loki.
- Dashboard personalizado en Grafana que muestre CPU, memoria, tráfico y logs.
- Alertas básicas definidas.

---

## 🎯 Mini-Quiz (respuestas al final)

1. ¿Cuál de estos NO es parte de la observabilidad?
   a) Métricas  
   b) Logs  
   c) Backups  

2. ¿Qué hace Prometheus?
   a) Gestiona usuarios  
   b) Recolecta y guarda métricas  
   c) Ejecuta contenedores  

3. ¿Qué es Loki?
   a) Herramienta de logs desarrollada por Grafana Labs  
   b) Base de datos relacional  
   c) Servidor web  

4. ¿Para qué sirve Promtail?
   a) Ver logs por consola  
   b) Enviar logs a Loki  
   c) Crear alertas  

5. ¿Qué archivo se usa para definir dashboards en Grafana?
   a) `dashboard.json`  
   b) `grafana.yaml`  
   c) `config.log`  

---

## 📺 Recursos Gratuitos

### Videos
- [¿Qué es Observabilidad? - DevTalles](https://www.youtube.com/watch?v=dnS3sSQ-LK8)
- [Prometheus explicado - DevTalles](https://www.youtube.com/watch?v=nP7pF8eyGvY)
- [Monitorización con Grafana y Prometheus - Midudev](https://www.youtube.com/watch?v=9iUeK0sx-PU)
- [Loki explicado - DevMentor](https://www.youtube.com/watch?v=CCmFgIPjeXY)

### Documentación
- https://prometheus.io/docs/introduction/overview/  
- https://grafana.com/docs/grafana/latest/getting-started/  
- https://grafana.com/docs/loki/latest/  
- https://www.cncf.io/blog/2020/12/10/observability-what-it-is-and-why-it-matters/

---

## ✅ Respuestas del Mini-Quiz

1. ✅ c) Backups  
2. ✅ b) Recolecta y guarda métricas  
3. ✅ a) Herramienta de logs desarrollada por Grafana Labs  
4. ✅ b) Enviar logs a Loki  
5. ✅ a) `dashboard.json`
