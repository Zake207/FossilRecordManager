# ADR 0004: Use of uvicorn as asgi

**Date:** 17-11-2025  
**State:** Accepted

## Context
Ensure the api selected has a good server that work with asynchronous querys with low latency and efficiency.

## Election
The chosen tool is *uvicorn*

## Considered Alternatives
- Hypercorn
- Daphne

## Consequences
### Good
+ Highly recomend when use *FastAPI*
+ Low latency
+ Work with websockets
### Bad
- Bad managing multiprocess
- Dont work perfectly with websockets

## References
- [Documentación oficial](https://uvicorn.dev/)