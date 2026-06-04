# Professional Dashboard V2 Visual Gap Audit

Generated: `2026-06-04T20:27:20Z`

## Local audit

- V1 exists: `True` size `1670188`.
- V1.5 exists: `True` size `1670188`.
- Chart existed, but it was still surrounded by data panels and the BUY/SELL word did not appear over the activation candle.
- WAIT/NOT_OPERABLE were visible as dashboard state, but not as a compact chart marker with clear no-active-trade semantics.
- Entry/stop/TP lines existed only for active trade, but labels were not TradingView-like enough: distance/R:R and long/short ordering needed clearer treatment.
- Future projection existed in V1.5 as scenario paths, but V2 needed explicit principal/alternative/invalidated semantics.
- Breakdowns were compact, but V2 requires dedicated TIMING/PRICE/CONFIRMATION/TRADE visual cards.
- Daily Stop was separated, but V2 makes it a mandatory Block B with the exact statistical-reference copy.

## Public audit

- Public URL opened: title Professional Allen Dashboard V1; visible text shows WAIT, summary/detail/forward/breakdowns before chart-dominant V2.

## Required V2 changes

- Cabina 44px top bar + watchlist + chart central dominant + panel derecho + bottom collapsible.
- BUY/SELL marker only when `active_trade=true`; WAIT/NOT_OPERABLE/NOT_AVAILABLE never draw active trade levels.
- TP/Stop/Hard Stop lines only for ACTIVE_LONG/ACTIVE_SHORT.
- Zone and timing bands remain visible for WAIT/NOT_OPERABLE when data exists.
- No fetch/websocket/localStorage/order/mutation APIs.
