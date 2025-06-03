# 📅 Semana 11 - Monitoreo, Logging y Alertas

## 🎯 Objetivo de la Semana
Aprender a implementar monitoreo, logging y sistemas de alertas para mantener la salud y rendimiento de aplicaciones e infraestructuras.

---

## 📘 Teoría

### 📊 Monitoreo con Prometheus y Grafana

- 🎥 [Introducción a Prometheus y Grafana - TechWorld with Nana](https://www.youtube.com/watch?v=h4Sl21AKiDg)
- 📘 [Documentación oficial de Prometheus](https://prometheus.io/docs/introduction/overview/)
- 📘 [Documentación oficial de Grafana](https://grafana.com/docs/grafana/latest/)
- ✅ *Práctica:* Configura Prometheus para recolectar métricas de un servicio y visualízalas con Grafana.

---

### 📚 Logging Centralizado con ELK Stack

- 🎥 [Introducción a ELK Stack (Elasticsearch, Logstash, Kibana) - Amigoscode](https://www.youtube.com/watch?v=R4nD9M9Qq3E)
- 📘 [Guía oficial de Elastic Stack](https://www.elastic.co/guide/index.html)
- ✅ *Práctica:* Configura un pipeline para enviar logs desde una aplicación a Elasticsearch y visualízalos en Kibana.

---

### 🚨 Sistemas de Alertas

- 🎥 [Alertmanager con Prometheus - DevOps Directive](https://www.youtube.com/watch?v=1FOz_LtILnk)
- 📘 [Alertmanager Documentation](https://prometheus.io/docs/alerting/latest/alertmanager/)
- ✅ *Práctica:* Crea reglas de alertas en Prometheus y configura notificaciones por correo o Slack.

---

## 🧪 Ejercicios

1. Instala Prometheus y Grafana localmente o en un contenedor.
2. Configura un exporter para monitorear métricas básicas (CPU, memoria).
3. Configura ELK Stack para centralizar logs.
4. Define reglas básicas de alertas en Prometheus y prueba las notificaciones.
5. Crea dashboards personalizados en Grafana para tu proyecto.

---

## 🛠 Proyecto: “Sistema de Observabilidad Completo”

**Objetivo:** Implementar un sistema integrado de monitoreo, logging y alertas para una aplicación contenerizada.

### Requisitos del Proyecto:

- Métricas recogidas con Prometheus y visualizadas en Grafana.
- Logs centralizados con Elasticsearch y visualizados en Kibana.
- Alertas configuradas con Alertmanager para eventos críticos.
- Documentación clara del setup y uso del sistema.

---

## 🎯 Mini-Quiz (respuestas al final del archivo)

1. ¿Qué herramienta se usa para visualizar métricas en esta semana?  
   a) Kibana  
   b) Grafana  
   c) Logstash  

2. ¿Cuál componente del ELK stack es responsable de la visualización?  
   a) Elasticsearch  
   b) Logstash  
   c) Kibana  

3. ¿Qué herramienta se usa para recolectar métricas?  
   a) Prometheus  
   b) Grafana  
   c) Alertmanager  

4. ¿Para qué sirve Alertmanager?  
   a) Visualizar métricas  
   b) Gestionar alertas y notificaciones  
   c) Almacenar logs  

5. ¿Cuál es una práctica recomendada al configurar alertas?  
   a) Ignorar alertas menores  
   b) Definir reglas claras y notificaciones rápidas  
   c) Deshabilitar alertas para evitar spam  

---

## 📺 Recursos Gratuitos

### Videos
- [Introducción a Prometheus y Grafana - TechWorld with Nana](https://www.youtube.com/watch?v=h4Sl21AKiDg)
- [Introducción a ELK Stack - Amigoscode](https://www.youtube.com/watch?v=R4nD9M9Qq3E)
- [Alertmanager con Prometheus - DevOps Directive](https://www.youtube.com/watch?v=1FOz_LtILnk)

### Documentación
- https://prometheus.io/docs/introduction/overview/
- https://grafana.com/docs/grafana/latest/
- https://www.elastic.co/guide/index.html
- https://prometheus.io/docs/alerting/latest/alertmanager/

---

## ✅ Respuestas del Mini-Quiz

1. ✅ b) Grafana  
2. ✅ c) Kibana  
3. ✅ a) Prometheus  
4. ✅ b) Gestionar alertas y notificaciones  
5. ✅ b) Definir reglas claras y notificaciones rápidas  
