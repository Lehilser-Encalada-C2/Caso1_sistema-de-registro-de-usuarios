Descripción del Caso:
El sistema debe permitir que un usuario cree una cuenta proporcionando datos básicos como nombre, correo electrónico, contraseña y otros campos requeridos 
según las necesidades. Además, debe garantizar la validación de datos, el almacenamiento seguro de la información, 
y el cumplimiento de políticas como el manejo seguro de contraseñas mediante cifrado. 
La finalidad es permitir que nuevos usuarios se registren en una plataforma y gestionen su información personal de manera segura y organizada.

Objetivo:
Implementar un sistema que permita registrar, almacenar y gestionar usuarios de forma segura y eficiente, 
garantizando la correcta validación de datos y el acceso autorizado a la plataforma.

Requerimientos Funcionales:
1.	Texto para indica al usuario que ubique su información personal.
2.	Diseño Gráfico.
3.	Mensaje de verificación si la información ingresada es correcta.
4.	Mensaje de notificación de inicio de sesión valida.
5.	Menú de inicio de la aplicación.
Requerimientos No Funcionales:
1.	Seguridad de la información.
2.	Rendimiento de carga de la página.
3.	Debe ser adaptable para distintos dispositivos.

Tabla de prueba:
|______________|______________|_____________________|____________________|_______________________________|__
|              |Requerimiento |                     |                    |	                             |
|              |asociado      |  Datos de entrada   | Resultado esperado | Resultado obtenido (simulado) |
|--------------|--------------|---------------------|--------------------|-------------------------------|--
| Prueba       |Registro de   | Nombre:             |El sistema registra | El sistema registro al usuario|   
| Unitaria 1	 |nuevo usuario | Jorge Sanunga.      |correctamente al    | y muestra mensaje "registro   |  
|              |              | Correo:             |usuario y muestra   | completado".                  |   
|              |              | jorgesanun@gmail.com|mensaje"registro    |                               |
|              |              | Contraseña: Sajo345 |completado".        |                               |
|--------------|--------------|---------------------|--------------------|-------------------------------|--                                                                                                           
|              | Inicio de    | Correo:             |El sistema permitirá|El sistema permite el acceso al|                                                  
|  Prueba      |  sesión      | jorgesanun@gmail.com|el acceso al usuario|usuario y redirige al principal|                                                                                       
| Unitaria 2   |              | Contraseña: Sajo345 |y redirige al menú  |                               |                                              
|              |              |                     |principal.          |                               |                         
|--------------|--------------|---------------------|--------------------|-------------------------------|--
| Prueba       |              | Correo:             |El sistema envía un |Ingrese a su correo para       |                                                             
| Unitaria 3   | Recuperación | jorgesanun@gmail.com|correo con enlace de|verificar su recuperación de   |                                                                                                        
|              |de contraseña |                     |recuperación.       |contraseña.                    |
|--------------|--------------|---------------------|--------------------|-------------------------------|--
| Prueba       | Seguridad    |                     |La contraseña debe  | En base de datos se almacena  |
| validación 1 |(contraseña   | contraseña: Sajo345 |almacenarse cifrada | y el sistema lo cifra, ejemplo|                                                                                                           
|              | sifrada)     |                     |en la base de datos,| (“$2b$12$XbW…”).              |                                                              
|              |              |                     |no en texto plano.  |                               |                              
|--------------|--------------|---------------------|--------------------|-------------------------------|--                                                                                                              
|              |Compatibilidad|Se ejecuta en Chrome,|El sistema debe     |El sistema opera sin errores en| 
| Prueba       |con los       |Firefox, Edge, Etc.  |funcionar           |todos los navegadores.         |                                                                                                    
|Validación 2  |navegadores   |                     |correctamente en    |                               |  
|              |              |                     |cualquier navegador.|                               |
|______________|______________|_____________________|____________________|_______________________________|__

Tipos de mantenimientos propuesto:
Caso 1:  Revisión de permisos, conexión y lógica de inserción de datos, además de depurar con herramientas específicas para detectar 
el punto exacto donde falla el guardado  (Adaptación Ambiental).

Caso 2:  Revisar el bloque de código, permisos y opción de recuperación de cuento, así como aspectos de seguridad  (Reparaciones de Fallas). 

Caso 3:  La aplicación puede tener un problema de conectividad o de ingreso con algunos dispositivos (Adaptiva). 
Si la app se actualiza desde un servidor se tiene que reiniciar la app para que todo funcione correctamente.

Reflexión sobre el control de versiones:
El control de versiones es una técnica como una práctica eficiente ya sea con un equipo de trabajo o solitario, esto permite resguardar el original y crear copias donde podemos trabajar 
y volver con el original si ocurre un error en las copias creadas.
