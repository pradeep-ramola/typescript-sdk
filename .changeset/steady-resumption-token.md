---
'@modelcontextprotocol/client': patch
---

Preserve the existing resumption token when a resumed Streamable HTTP SSE stream closes before receiving another event id. Reconnects now continue sending the same `Last-Event-ID` instead of dropping it and accidentally opening a fresh stream.
