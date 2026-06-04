# Professional Dashboard V1 Visual QA Fix

Generated: 2026-06-03T23:19:08Z

## Scope

Corrección visual/UX del dashboard profesional V1. No se recalculan datos, no se cambian señales, stops, TP, pesos, trading ni snapshots productivos.

## Cambios

- Chart central con altura mínima desktop y layout menos comprimido.
- NOT_OPERABLE/WAIT deja de tapar el gráfico y pasa al panel de decisión.
- Separación explícita entre Señal actual y Daily Stop Model.
- Breakdown avanzado convertido a tablas legibles; no se muestra JSON crudo.
- Cabecera del chart explica que STRONG_OK del Daily Stop es estadístico y no orden operable.
- Bottom panel reorganizado con cards y details colapsables.

## ES Visual State

- Activo: ES / SP500
- Señal actual: WAIT
- Operable: False
- Daily Stop Model: STRONG_OK
- Interpretación: El modelo diario de stop para ES es fuerte, pero la señal actual está en espera. No hay operación activa hasta que Allen valide trigger/confirmación.

## Executive Answers

1. Se veía mal el gráfico: si, podía comprimirse y quedar interferido por overlays.
2. Render del gráfico corregido: si, chart central con min-height 580px y layout vertical menos comprimido.
3. JSON crudo visible eliminado: si, breakdowns convertidos a tablas legibles y colapsables.
4. Señal actual separada de Daily Stop Model: si.
5. NOT_OPERABLE movido: si, ya no tapa el chart; aparece como estado en panel derecho.
6. ES muestra WAIT sin confundirlo con STRONG_OK: si, ES actual=WAIT y Daily Stop=STRONG_OK.
7. Chart con altura correcta: si, min-height 580px en desktop.
8. Panel derecho legible: si, incluye bloque Señal actual y Daily Stop separado.
9. Panel inferior legible: si, resumen + detalle + breakdowns colapsables.
10. Capas siguen funcionando: si, controles conservados.
11. Carga los 14 activos: si.
12. Dashboard sigue read-only: si.
13. Dashboard calcula algo: no.
14. Fetch/websocket/localStorage: no.
15. Producción intacta: si.
16. shadow_only sigue activo: si.
17. Capturas generadas: no, sin renderer Playwright/Chrome/Chromium disponible.
18. Pendiente V2: validación visual con navegador real, posible motor de chart dedicado y refinamiento responsive fino.
19. Archivos modificados: reports/dashboard/professional_allen_dashboard_v1.html, reports/dashboard/explainable_allen_dashboard.html, reports/dashboard/explainable_sheets y builder scripts/build_professional_dashboard_v1.py.
20. Backup: reports/dashboard/backups/professional_allen_dashboard_v1_before_visual_qa_YYYYMMDD_HHMMSS.html.

## Policy

shadow_only = true
production_signals_modified = false
production_weights_modified = false
automatic_trading = false
classic_predictor_replaced = false
neural_promotion = false
dashboard_calculates_signals = false
dashboard_modifies_data = false

Listo para auditoría ChatGPT.
