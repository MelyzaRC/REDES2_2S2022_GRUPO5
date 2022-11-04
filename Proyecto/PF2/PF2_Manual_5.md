><img src="https://upload.wikimedia.org/wikipedia/commons/4/4a/Usac_logo.png" alt="drawing" width="75">
>
>Universidad San Carlos de Guatemala
>
>Facultad de Ingeniería 
>
>Escuela de Ciencias y Sistemas 
>
>Segundo Semestre, 2022
>
>Laboratorio de Redes de Computadoras 2 

### Grupo No.5

Integrantes:

| Nombre                               | Carnet    |
| ------------------------------------ | --------- | 
| <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRH6Uyi30Ty2WkMb0ZjuFLoXmkRwrrMObm-X2zztWtGbOgyA-i7mFzuiSKltN14HLAJDVM&usqp=CAU" alt="drawing" width="20"> &nbsp;Jimmy Yorbany Noriega Chávez         | 200915691 |
|  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQvke8Pr8T6xz52yM8v0ieg0oQy9L9SwfkO4hy4IKoRpxyQBKSGUWto7sWmzj9YYgm1VzU&usqp=CAU" alt="drawing" width="20"> &nbsp; Melyza Alejandra Rodríguez Contreras | 201314821 |
| <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRH6Uyi30Ty2WkMb0ZjuFLoXmkRwrrMObm-X2zztWtGbOgyA-i7mFzuiSKltN14HLAJDVM&usqp=CAU" alt="drawing" width="20"> &nbsp; Romael Isaac Pérez Godinez           | 201213545 | 
| <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRH6Uyi30Ty2WkMb0ZjuFLoXmkRwrrMObm-X2zztWtGbOgyA-i7mFzuiSKltN14HLAJDVM&usqp=CAU" alt="drawing" width="20"> &nbsp; Josué Alfredo González Caal          | 201602489 | 

# Proyecto - Fase 2

## Contenido
- Implementacion de ACLs para controlar el tráfico en las subredes 

## Implementacion de ACLs para controlar el tráfico en las subredes 
> ¿Qué es una ACL?
> 
> Por sus siglas en inglés ***access control list***, una ***lista de control de acceso*** es un concepto de seguridad informática usado para fomentar la separación de privilegios. Es una forma de determinar los permisos de acceso apropiados a un determinado objeto, dependiendo de ciertos aspectos del proceso que hace el pedido.
> 
> Las ***ACL*** permiten controlar el flujo del tráfico en equipos de redes, tales como enrutadores y conmutadores. Su principal objetivo es filtrar tráfico: permitir o denegar el tráfico de red de acuerdo con alguna condición. Sin embargo, también tienen usos adicionales, como, por ejemplo, distinguir "tráfico interesante" (tráfico suficientemente importante como para activar o mantener una conexión) en RDSI (red digital de servicios integrados).
> 
> ![ACL](images/acl.png "Ilustración ACL")

### Pasos para configurar una lista de control de acceso en AWS
1. Ingresar al **Panel VPC** dentro de la consola de AWS

![PASO1](images/1vpc.PNG "Panel VPC")

2. En el apartado de **Seguridad** (ubicado en el panel de navegación izquierdo), seleccionar la opción **ACL de red**.

![PASO2](images/2seguridad.png "Apartado seguridad")

3. Seleccionar la opción ***CREAR ACL DE RED***.

![PASO3](images/3crear.png "Opcion crear")

4. Colocar un nombre y seleccionar una VPC para crear la nueva lista de control de acceso. Posteriormente, hacer click en la opción **CREAR**, en la parte inferior de la pantalla. 

![PASO4](images/4rellenar.PNG "Llenar informacion")

Una vez realizado este paso, podemos observar que se ha creado la nueva ACL. 

![PASO41](images/5mostrar.PNG "Mostrar nuevas acls")

5. Seleccionar la ACL que se creo anteriormente. 

![PASO5](images/6seleccionar.PNG "Seleccionar ACL creado")

Ahora, podemos editar las reglas, tanto de entrada como de salida, a nuestra conveniencia. 

### Creación de una regla de entrada
1. Ubicarse en la pestaña **Reglas de entrada** (dentro de la ACL creada) y hacer click sobre el botón **Editar reglas de entrada**.

![PASO6](images/7.png "Crear regla de entrada")

2. Seleccionar la opción **Crear nueva regla** y rellenar todos los campos que se solicitan. 

![PASO7](images/8.PNG "Crear regla y rellenar campos")

3. Guardar los cambios y verificar la creación de la regla de entrada. 

![PASO8](images/9.PNG "Guardar y revisar")

### Creación de una regla de salida 
1. Ubicarse en la pestaña **Reglas de salida** (dentro de la ACL creada) y hacer click sobre el botón **Editar reglas de salida**.

![PASO9](images/10.PNG "Crear regla de salida")

2. Seleccionar la opción **Crear nueva regla** y rellenar todos los campos que se solicitan. 

![PASO10](images/11.PNG "Crear regla y rellenar campos")

3. Guardar los cambios y verificar la creación de la regla de salida. 

![PASO11](images/12.PNG "Guardar y revisar")
