# 📚 Guía por fases — Workshop Observabilidad sin humo

Este documento organiza el workshop en fases didácticas, cada una con objetivos claros, archivos involucrados y validaciones reales. Está diseñado para facilitar la enseñanza, el seguimiento y la evolución del proyecto.

---

## 🧩 Fase 1 — Stack reproducible

**Objetivo:**  
Levantar Prometheus, Grafana, Alertmanager y Node Exporter con Docker Compose

**Archivos clave:**

- `docker-compose.yml`
- `prometheus/prometheus.yml`
- `grafana/datasources/datasource.yml`
- `grafana/dashboards/node.json`
- `grafana/dashboards/dashboard.yml`
- `alertmanager/config.yml`

**Validaciones:**

- ✔ Servicios activos en sus puertos
- ✔ Dashboards cargados automáticamente
- ✔ Conectividad entre servicios

---

## 🧩 Fase 2 — Simulación de alertas

**Objetivo:**  
Configurar alertas reales en Prometheus y visualizarlas en Grafana

**Archivos clave:**

- `prometheus/alert.rules.yml`
- `scripts/test-alert.sh`
- `scripts/debug.sh`

**Validaciones:**

- ✔ Alerta `HighLoad` disparada
- ✔ Estado `alerting` visible en Grafana
- ✔ Panel de alerta activo en el dashboard

**Corrección aplicada:**  
Umbral ajustado a `avg(node_load1) > 0.1` para entornos livianos

---

## 🧩 Fase 3 — Validación y documentación

**Objetivo:**  
Registrar errores, correcciones y mejoras como parte del aprendizaje

**Archivos clave:**

- `README-TEST.md`
- `README-STEPS.md`
- `README-FACILITADOR.md`

**Validaciones:**

- ✔ Documentación actualizada con cada corrección
- ✔ Scripts funcionales y didácticos
- ✔ Flujo reproducible y listo para enseñar

---

## 🧩 Fase 4 — Buenas prácticas y presentación

**Objetivo:**  
Modelar estándares profesionales y preparar el proyecto para compartir

**Archivos clave:**

- `.dockerignore`
- `README.md`
- `README-FINAL.md`

**Validaciones:**

- ✔ Exclusión de archivos innecesarios en contexto de build
- ✔ Documentación clara y atractiva
- ✔ Listo para reclutadores y comunidad

---

