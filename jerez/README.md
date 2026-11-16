# Dashboard Fidelización JEREZ

Destino fuente Dropbox: ns:645300720//DASHBOARD JEREZ 2026. Independiente de SC. HTML en jerez/index.html; publicar solo jerez, nunca estado privado. Creado16/11/2026. Misma identidad C4 y diez secciones. Primera estructura con estadísticas disponibles; filtros interactivos, gráficos semanales, comparaciones30vs30, totalesonboarding y actualización diaria pendientes de completar. No afirmar equivalencia funcional completa aún.

SOCIOS.xls id:vZMJ-le_tQ0AAAAAAABN2Q client_modified2026-11-16T12:54:20Z216576bytes. Cabecera Codigo,F.Nacimiento,Sexo,Fechaalta,Cuota/inicio/fin4/5/6,Cuota7/inicio9/fin10(columna8vacía),Cuota3/inicio12/fin13. Localizar cabeceras y posicionesduplicadas; excluir porconceptoTOALLAS/SEGURO/NO REACTIVAR, vigenteinicio<=corte<=fin(oabierto).959códigos vigentes de1163filas;204sinabono vigente confirmado. No equivale abaja. Sexo/nacimiento solo paraagregados no persistir individualmente. Un solo grupoJEREZ, no copiarESADE/SC. FaltaBAJAS: total segúnlistado yvigencia, no bajasefectivas certificadas.

ACCESOS1.8.26A16.11.26.xls id:vZMJ-le_tQ0AAAAAAABN2g5712384bytes client12:57:13Z. Descargaroriginal (más5MiB), fechasExcel reales, horaTEXTOHH:MM sinsegundos no inventarprecisión.784coincidenciasexactas codigo/fecha/hora/sentido a precisiónfuente, advertir repeticiónenmismo minuto puede ser indistinguible. SoloEntrada métricas, visita díadistinto. Cobertura01/08–16/11parcial sin díasvacíos.169ausencia14convisitaconocida,47sinvisitaobservada; no interpretar ausenciaobservada como inactividad.

Historico/estado-jerez-2026-11-16.json privado mínimo sinnombre/nacimiento/sexo. Preservarversiones ycontactos, acumularaccesos deduplicados sinborrar anteriores. No nuevo corte por ejecución. No datos identificativos enGitHub/web. No enlaces públicosDropBox.

Fuentes pendientes:BAJAS.xls,AADD,Ingresos2026,Presupuesto2026.xlsx,históricosocios,seguimientoinicial,satisfacción,incidencias,objetivos,renovaciones,motivosbaja. MantenerPendiente no0. No inferir gruposni clasificar cuotas deJerez segúnSC. Conservarúltimoestadoválido siarchivofalta. Se creará/activaráactualizacióndiaria solo cuando importador ypublicación estén validados.


## Fuentes incorporadas16/11: ingresos,presupuesto,histórico
Ingresos/ene.xls…oct.xls (client16/11/2026) completos: localizarB.Imponible/IVA/TOTAL porcabecera15columnas, validar base+IVA=totalcon1céntimo. Sumar baseencéntimos, negativos incluidos, excluir subtotales por descripción vacía. Clasificación porgrupo:CUOTAS/PRORRATASDECUOTAS/BONOSDECUOTAS=>Cuotas salvoTOALLAS/SEGURO=>Varios;CURSILLOS=>Cursos;otrosVarios. Presupuestohoja2026: fila2Cuotas,fila7Cursos(subtotal,NOvolverasumarfila3–6),fila12IngresosTOTAL;Varios=TOTAL−Cuotas−Cursos(incluyePádel,piscinaexterior,campus,varios). Fiscalpresupuestoindeterminado,sintransformar. Realenero–octubre586879.91€,presupuestoanual720823.50€,diferencia−133943.59€,81.4%. Nov/dicrealnullPendiente, not0. Cuadroinicial3categorías+TOTALy detallemensual, soloagregadosincomeData.
Histórico socios y cursillistas hasta octubre2026.xlsx hojaSOCIOS:bloques2018–2026 conaño,col1–12meses,siguientesfilasSocios/Cursillistas/total.Validarsuma,omitirmeses2026novdicvacíos.106puntos2018-01…2026-10,último1169socios+528cursillistas1697. Preservarcategoríasoriginales,no confundir con959cuotasvigentes16/11;no inferirbajas. memberHistoryData.monthly. BackupprivadoagregadoHistorico/agregados-finanzas-historico-2026-11-16.json. Ingresos/presupuesto/histórico ya disponibles: sustituye estado pendientes anterior. Aúnpendientesgráficosyfiltrosinteractivos,BAJAS,AADD,seguimiento. No restaurarversionessindatosnuevos.


## Clasificación ingresos confirmada Paloma16/11 (prevalece)
VARIOS: concepto normalizado VINILO MEDAC (MENSUAL), BONO 10 ENTRADAS (10 SESIONES), y gruposARTICULOS/ARTÍCULOS,TAQUILLAS,MATRICULAS/MATRÍCULAS. CURSOS: grupoCURSILLOS. Todos los demás movimientos=>CUOTAS. Aplicar por movimiento, mayúsculas/trim, preservar negativos y baseSINIVA. No usar reglaSC, no excluir automáticamenteSEGURO/TOALLASdeingresos si no están enVARIOS segúnesta lista. Reglas deuniversosocios sonindependientes. Presupuesto originalsin reclasificación nueva: conservarvaloresprevios de fuente. Totalesmensualesy586879.91€global intactos. BackupnuevoHistorico/agregados-reclasificados-2026-11-16.json preserva anterior. Mantenerregla cadaactualización.


Colores confirmados16/11: en evolución histórica, Clientes (socios de fuente) verde #16a34a y Cursillistas rojo #dc2626, tanto encabezados como cifras. Totales neutros. Conservar en próximas actualizaciones.
