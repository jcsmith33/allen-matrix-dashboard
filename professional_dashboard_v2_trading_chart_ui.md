# Professional Dashboard V2 - Trading Chart Signal UI

Generated: 2026-06-04T20:27:21Z

## Outputs

- V2: `/mnt/c/allenmatrix/reports/dashboard/professional_allen_dashboard_v2.html`
- V1 actualizado: `/mnt/c/allenmatrix/reports/dashboard/professional_allen_dashboard_v1.html`
- Explainable dashboard actualizado: `/mnt/c/allenmatrix/reports/dashboard/explainable_allen_dashboard.html`
- Index actualizado: `/mnt/c/allenmatrix/reports/dashboard/index.html`
- Backup: `/mnt/c/allenmatrix/reports/dashboard/backups/professional_allen_dashboard_before_v2_20260604_222720.html`
- Visual gap audit: `/mnt/c/allenmatrix/reports/research/professional_dashboard_v2_visual_gap_audit.md`
- Validation CSV: `/mnt/c/allenmatrix/reports/research/professional_dashboard_v2_validation.csv`

## Estado por activos prioritarios

- ES: NOT_OPERABLE active_trade=False DailyStop=STRONG_OK
- NQ: NOT_OPERABLE active_trade=False DailyStop=STRONG_OK
- FDAX: NOT_OPERABLE active_trade=False DailyStop=STRONG_OK
- RTY: NOT_OPERABLE active_trade=False DailyStop=STRONG_OK
- YM: NOT_OPERABLE active_trade=False DailyStop=OK
- GC: ACTIVE_SHORT active_trade=True DailyStop=OK
- CL: NOT_OPERABLE active_trade=False DailyStop=OK

## Activos sin modelo Daily Stop

SI, HG, QG, SPX, VX, US30Y, PLG

## Capturas

Capturas no generadas por falta de renderer.

## Respuestas ejecutivas

1. ¿El gráfico es ahora el elemento dominante? Sí: watchlist izquierda, chart central dominante y panel derecho compacto.
2. ¿BUY aparece sobre la vela cuando hay señal activa? Sí, lógica ACTIVE_LONG implementada. Activos actuales: ninguno.
3. ¿SELL aparece sobre la vela cuando hay señal activa? Sí, lógica ACTIVE_SHORT implementada. Activos actuales: GC.
4. ¿WAIT deja de mostrar trade activo? Sí: los niveles de trade se dibujan solo con isActiveTrade(r).
5. ¿NOT_OPERABLE deja de mostrar trade activo? Sí.
6. ¿TP1/TP2/TP3 se dibujan correctamente? Sí, solo en ACTIVE_LONG/ACTIVE_SHORT con etiquetas, precio, distancia y R si existe.
7. ¿Stop y hard stop se ven claramente? Sí, stop rojo y hard stop/invalidación rojo intenso.
8. ¿La zona de giro se ve claramente? Sí, banda horizontal translúcida con estado y distancia.
9. ¿La ventana temporal se ve claramente? Sí, banda vertical translúcida con rango y fecha central si existe.
10. ¿Hay proyección futura principal/alternativa/invalidada? Sí, desde última vela usando escenarios existentes; si faltan se muestra no disponible.
11. ¿Daily Stop Model queda separado de señal actual? Sí, Bloque A señal actual y Bloque B Daily Stop Model.
12. ¿Los breakdowns son legibles? Sí, tarjetas TIMING/PRICE/CONFIRMATION/TRADE sin JSON crudo.
13. ¿Se redujo el scroll inicial? Sí, layout 100vh con bottom compacto y debug cerrado.
14. ¿Cargan los 14 activos? Sí.
15. ¿Dashboard sigue read-only? Sí.
16. ¿Dashboard calcula algo? No calcula señales/stops/TP; solo transforma visualmente campos existentes.
17. ¿Producción quedó intacta? Sí.
18. ¿shadow_only sigue activo? Sí.
19. ¿Qué falta para V3? Capturas con renderer real, test visual cross-viewport, posible librería lightweight-charts si se autoriza dependencia.
20. ¿Dónde está el backup? /mnt/c/allenmatrix/reports/dashboard/backups/professional_allen_dashboard_before_v2_20260604_222720.html

## Política final

shadow_only = true
production_signals_modified = false
production_weights_modified = false
automatic_trading = false
classic_predictor_replaced = false
neural_promotion = false
dashboard_calculates_signals = false
dashboard_modifies_data = false

Listo para auditoría ChatGPT.
