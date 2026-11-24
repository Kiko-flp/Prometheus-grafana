# 6. Pruebas de carga del servidor

Sección para generar carga controlada en el servidor y comprobar cómo se reflejan los cambios en Prometheus y Grafana.

## 6.1 Generación de carga con `stress` / `stress-ng`

```bash
stress --cpu 2 --timeout 60s
```

| Parámetro | Descripción |
| --- | --- |
| `--cpu 2` | Lanza dos procesos para saturar dos núcleos de CPU. |
| `--timeout 60s` | Mantiene la prueba de carga durante 60 segundos. |
