# SqlSpringSecurityDefaultSchema
Esquema sql básico para poder integrarse con spring security en un app de roles
Tiene una tabla user y una tabla authorities y un campo username relaciona ambas tablas,
éste username sería la calve foránea de authorities a user.
La aplicación montada sobre este esquema tendría dos roles ( "ADMINISTRADOR" y "SUPERVISOR") 
de quere añadir más lo único que habría que hacer sería añadirlos al camo authority de la tabla
authorities
Este esquema básico no contempla la encriptación de la contraseña por ello están los valores
del campo password con {noob} para que ignore la encriptación que es un requisito de spring security
, de todas maneras, esto an algunos getores de sql puede fallar y tendríamos que incorporar 
un password encoder en Java
