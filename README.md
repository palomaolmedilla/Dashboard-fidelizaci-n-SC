# Dashboard Fidelización SC

Dashboard público de estadísticas agregadas, publicado en https://dashboard-fidelizacion-sc.onrender.com/ mediante Render Static Site.

## Actualización
La tarea ChatGPT Actualizar fidelización SC consulta SOCIOS.xls y ACCESOS.xls en Dropbox /C4 CONTROL/DASHBOARD FIDELIZACIÓN SC y actualiza index.html. El resumen agregado se encuentra en la constante summary. No publicar datos individuales ni identificadores en este repositorio público. Conservar el diseño e interacciones al sustituir el resumen. Los datos actuales sustituyen la demostración desde 01/11/2026.

## Reglas
SOCIOS tiene encabezados Cuota duplicados: columnas 4, 6, 7 (base cero). Ignorar conceptos TOALLAS y SEGURO. Conservar una sola persona si otra cuota no adicional está listada. Esta selección no acredita vigencia de cada cuota. Fecha de baja efectiva al corte excluye al socio del total activo.

Asistencia: solo Entrada, deduplicar por código, fecha, hora, sentido; cruzar códigos con abono listado. Entrada no equivale a día de visita. Socios únicos se deduplican por mes. No reconstruir cuotas históricas desde cuotas actuales.

Las fechas extraídas de los XLS están en mes/día/año; validar contra los encabezados y fechas no ambiguas. El 01/11/2026 es parcial. Días sin registros en el histórico actual: 22 y 23 agosto, 4 octubre; marcar incertidumbre sin asumir cierre. Comparación publicada: 02/10–31/10 frente a 02/09–01/10, socios activos cuya alta es ≤ 02/09 y al menos una entrada en la ventana previa. Inactividad solo observada; sin entradas en histórico se separa.

No calcular tasas de bajas, retención o bienvenida si faltan datos. No inventar ceros. Actualizar cobertura, fechas y período parcial en cada publicación. Render despliega main automáticamente: consultar list_deploys antes de intentar un despliegue manual, verificar commit live y sitio público.

## Ocho áreas (01/11/2026)
El dashboard contiene asistencia, primeros 30–90 días, antigüedad, clases, experiencia, objetivos, cuotas/renovación y motivos de baja. Actualizar la constante dashboardData de index.html, no summary. Conservar todas las secciones.

Visitas ahora significa días distintos con Entrada por socio; entradas al torno es otra medida. Recuento de caída de frecuencia por días de visita: 210 / 953 (antes, 218 por movimientos). Actualizar ventanas, rótulos, fechas y explicaciones al cambiar el corte.

Datos agregados: attendance (monthly/weekly/gaps/comparison), onboarding (grupos actuales y señal de 4 días en primeros 30 entre altas con ventana completa), tenure (distribución actual), fees (conceptos no excluyentes, fechas de baja futuras sin asumir renovación), bajas (cobertura y ausencia de motivos). Ver definiciones en el HTML. No presentar supervivencia/retención a partir de población actual.

Fuentes adicionales pendientes: SEGUIMIENTO_INICIAL.csv; CLASES.csv; SATISFACCION.csv e INCIDENCIAS.csv; OBJETIVOS.csv; RENOVACIONES.csv; BAJAS_MOTIVOS.csv. Hay plantillas vacías descargables para recoger datos. No hay importador de estas nuevas fuentes todavía: al aparecer, validar primero su estructura y ampliar el cálculo sin exponer información individual ni inventar métricas. No representar ausencia de fuente como cero.

## AADD: agrupación y exploración (02/11/2026)
La sección 05 usa `aaddData` con sesiones agregadas de los Excel AADD y `aaddGroups` para clasificar actividades. Mantener la primera fila de resumen en «Explorar las actividades» (corrección expresa de Paloma). Ofrecer filtro de grupo y desplegables por grupo con métricas recalculadas desde sesiones validadas, conservando filtros de mes, sala y búsqueda. CUERPO/MENTE: YOGA, YOGA VINYASA, PILATES, PILATES/STRETCHING, HIPOPRESIVOS/PILATES, STRETCHING, YOGA FUERZA. CARDIO: CYCLING, CLUB DEL CORREDOR y MASTERCLASS CYCLING. BAILE: ZUMBA, ZUMBA 30', COOL DANCE. TONO: TBC, TONO 30', GAP, C4 PUMP. FUERZA: CROSS4U, POWER INTERVAL, HYBRID, FUERZA, HIIT-CORE. Conservar actividades nuevas como «Sin clasificar» hasta poder clasificarlas, sin descartarlas. No publicar empleado, NIF ni observaciones. Sin identificación de asistentes no aplicar desglose ESADE/SC, sexo o edad a estas fuentes. Espera vacía no implica cero; valoración es media simple por sesión; asistencia son participaciones, no personas únicas.
