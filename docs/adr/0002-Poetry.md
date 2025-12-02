# ADR 0002: Use of poetry as package manager

**Date:** 10-11-2025  
**State:** Accepted

## Context
The project needs to manage the python modules to be operative in every system and register the dependencies of the project

## Election
The manager this project will use is *poetry*

## Considered Alternatives
- virtual enviorment: basic and useful but I decided to explore new technologies
- uv: similar, not discarted at all but prefered to use poetry
## Consequences
### Good
+ Allow to instantiate the dependencies of the project
### Bad
- Must spend time learning how to configure it

## References
- [Documentación oficial](https://python-poetry.org/docs/)