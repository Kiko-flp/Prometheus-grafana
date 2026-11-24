# 4. Añadir Prometheus como fuente de datos

Para que Grafana pueda consultar las métricas almacenadas por Prometheus, es necesario añadirlo como *Data Source*.

## 4.1 Pasos de configuración

1. Accede en Grafana a **Connections > Data sources > Add data source**.
2. Selecciona **Prometheus**.
3. Indica la URL del servidor Prometheus (por ejemplo, `http://localhost:9090`).
4. Pulsa **Save & test** para comprobar la conexión.

| Campo | Valor |
| --- | --- |
| **Type** | `Prometheus` |
| **Prometheus server URL** | `http://localhost:9090` |
