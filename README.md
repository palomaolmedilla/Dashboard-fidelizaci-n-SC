# Dashboard Fidelización SC

Dashboard público de estadísticas agregadas, publicado en https://dashboard-fidelizacion-sc.onrender.com/ mediante Render Static Site.

## Actualización
La tarea ChatGPT Actualizar fidelización SC consulta SOCIOS.xls y ACCESOS.xls en Dropbox /C4 CONTROL/DASHBOARD FIDELIZACIÓN SC y actualiza index.html. El resumen agregado se encuentra en la constante summary. No publicar datos individuales ni identificadores en este repositorio público. Conservar el diseño e interacciones al sustituir el resumen. Los datos actuales sustituyen la demostración desde 01/11/2026.

## Reglas
SOCIOS tiene encabezados Cuota duplicados: columnas 4, 6, 7 (base cero). Ignorar conceptos TOALLAS y SEGURO. Conservar una sola persona si otra cuota no adicional está listada. Esta selección no acredita vigencia de cada cuota. Fecha de baja efectiva al corte excluye al socio del total activo.

Asistencia: solo Entrada, deduplicar por código, fecha, hora, sentido; cruzar códigos con abono listado. Entrada no equivale a día de visita. Socios únicos se deduplican por mes. No reconstruir cuotas históricas desde cuotas actuales.

Las fechas extraídas de los XLS están en mes/día/año; validar contra los encabezados y fechas no ambiguas. El 01/11/2026 es parcial. Días sin registros en el histórico actual: 22 y 23 agosto, 4 octubre; marcar incertidumbre sin asumir cierre. Comparación publicada: 02/10–31/10 frente a 02/09–01/10, socios activos cuya alta es ≤ 02/09 y al menos una entrada en la ventana previa. Inactividad solo observada; sin entradas en histórico se separa.

No calcular tasas de bajas, retención o bienvenida si faltan datos. No inventar ceros. Actualizar cobertura, fechas y período parcial en cada publicación. Render despliega main automáticamente: consultar list_deploys antes de intentar un despliegue manual, verificar commit live y sitio público.
