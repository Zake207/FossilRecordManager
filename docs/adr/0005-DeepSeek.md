# ADR 0005: Use of deepseek as ai assistant

**Date:** 17-11-2025  
**State:** Pending

## Context
It would be interesting to implement a chatbot that helps the user in simple tasks, but develop a new ai is a brand new project that cosumes a lot of time to train for the especific context this application has, so the final option is to use generic model and give it a full context of its task.  

## Election
The ai engine is *deepseek/deepseek-r1:free* in *openrouter*

## Considered Alternatives
- develop a genuine ai
- mistralai/mistral-7b-instruct:free
- microsoft/mai-ds-r1:free
- openrouter/auto
## Consequences
### Good
- very easy to give context and generic
### Bad
- maybe has some limitation in the task it can handle
- it has a limited use for that api key so is not consistent for a large aplication


## References
- [Documentación oficial](https://openrouter.ai/deepseek/deepseek-r1:free)