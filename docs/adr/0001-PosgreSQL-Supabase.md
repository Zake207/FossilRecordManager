# ADR 0001: Use of Postgres as DataBase

**Date:** 10-11-2025  
**State:** Accepted

## Context
The project needs a powerful database but, as a economic product, it is not planned to spend money on it.

## Election
The DataBase this project is going to use as a solution is *PostgreSQL* using *SupaBase*, for the image storage it will use Supabase Storage

## Considered Alternatives
- SQL: Don't allow me to explore other alternatives
- SQLite: Non-realistic option in the hypothetycal scenary where this is a massive project, is not scalable.
## Consequences
### Good
+ Learn a realistic tool
+ Develop using a already stablished database server
+ Use a interactive and visual interface
### Bad
- Need internet to connect to the database
- Must spend time learning how to configure it
- Maybe too complex for this case

## References
- [Documentación oficial (PostgreSQL)](https://www.postgresql.org/docs/)
- [Documentación oficial (Supabase)](https://supabase.com/docs)