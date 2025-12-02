## Entities of the DataBase

### USER
+ <u>user_id</u>
+ nickname
+ email
+ contraseña_hash

### RECORD
+ <u>record_id
+ user_id</u>
+ scientific_name
+ creation_date
+ notes
+ taxonomy
+ images[]

### IMAGE
+ <u>id
+ registro_id</u>
+ url_archivo