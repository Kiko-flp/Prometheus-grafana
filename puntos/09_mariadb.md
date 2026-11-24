# 9. Monitorización de bases de datos MariaDB

Ejercicio dedicado a la monitorización de bases de datos **MariaDB** mediante el exportador `mysqld_exporter`.

## 9.1 Flujo de configuración

1. Crear un usuario específico en MariaDB con permisos mínimos de monitorización (`PROCESS`, `REPLICATION CLIENT`, `SELECT`).
2. Configurar y arrancar `mysqld_exporter` (puerto por defecto `9104`).
3. Añadir el nuevo *job* en `prometheus.yml` apuntando al puerto `9104`.
4. Importar o crear un panel en Grafana para visualizar conexiones, consultas y estado del servidor.
