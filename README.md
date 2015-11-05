# CONVOCATORIA:

EONCORE se complace en convocar a cualquier persona dentro de la empresa (sin contar a los jefes de desarrollo) al Innovation Challenge v1.0, el cual busca promover los valores de competitividad, autoaprendizaje, investigacion e innovacion en beneficio del crecimiento profesional y laboral de cada uno de los involucrados y por ende de la empresa misma.

El objetivo final sera desarrollar un prototipo funcional de sistema web que sirva como base del **"Sistema Interno de Informacion"**, util como herramienta diaria de trabajo en las labores de todas a las areas de la empresa.

---

## BASES:

1. Deberan participar de manera individual y sin asesoria de ningun personal a cargo.
2. Es de caracter obligatorio para el personal de Desarrollo y opcional para el resto de los departamentos.
3. Se dara obligatoriamente 1 hora de horario laboral minimo, cada uno de los dias laborales a partir del dia 4 de Noviembre y hasta el Jueves 3 de Diciembre.
4. Las instalaciones de EONCORE estan disponibles para el desarrollo de los proyectos las 24 horas de los fines de semana, asi como de 6:00 PM a 9:00 AM entre semana.


## REQUERIMIENTOS TECNICOS MINIMOS:

 1. Tecnologias Requeridas:
   2. **AngularJS 1.4+.** (Recomendado 1.5)
   3. **NodeJS	0.11+.** (Recomendado 4.0+)
   4. Bases de Datos permitidas:
     5. **MySQL / MariaDB**
     6. **MongoDB**
     7. **RethinkDB**
     8. **FireBase** (Solo Database)
   5. **Bootstrap 3+**
   6. **Angular Material**
   7. Repositorio publico en **GitHub**

 2. Tecnologias de Valor Extra:
     1. **Gulp:** Para automatizacion de la implementacion.
     2. **Bower:** Para manejo de dependencias FrontEnd.
     3. **NPM:** Hacer modulo de Node una o mas partes del proyecto.
     4. Captcha Avanzado: Elementos de Autenticacion por Audio o Interaccion, diferente a Imagenes con caracteres obfuscados. 

 3. Caracteristicas del Proyecto (Casos de Uso):

####  Caso 1:
El sistema debera ser tipo Panel con acceso por Autenticacion con cuenta de Correo y Password.

####  Caso 2:
Las cuentas de usuario deberan ser almacenadas en BD, el password debera ser encriptado con algoritmos no reversibles, asi como almacenar bitacora de accesos.
	
####  Caso 3:
El sistema requiere Control de Acceso (ACL) con tabla de permisos y asignacion por usuario.
	
####  Caso 4:
El panel debera tener una area de Menu, la cual debera tener opciones dinamicas, generadas a partir de BD y registros de Modulos activos.

####  Caso 5:
Debera desarrollarse un modulo (de aqui en adelante MODULO DE TAREAS) para el registro de la Bitacora de Tareas, que permita crearlas, editarlas, borrarlas y consultarlas. 

####  Caso 6: 
Cada tarea debera poderse dar de alta con 3 datos minimos, 1 capturado por el usuario, que es el Titulo, los otros datos minimos requeridos tendran valor por default:
 1. Titulo (Obligatorio capturado)
 2. Fecha y Hora de Creacion (Obligatorio por default): Sera igual a la fecha y hora de creacion hasta que el usuario decida alterar este campo y asignar otra fecha-hora de inicio de la tarea.
 3. Usuario que Creo la Tarea (Obligatorio = Usuario de la Sesion activa).

####	Caso 7:
Cada tarea debera ser de 1 solo tipo dentro de los 3 posibles, que son:
 - TAREA (Planificada).
 - MEJORA (Propuesta libre).
 - FIX (Correccion de Error).

#### 	Caso 8:
Cada tarea tendra mas campos opcionales, que podran ser agregados en forma de captura/edicion ampliada, los cuales son:
 - Descripcion 
 - Fecha y Hora de Terminado
 - Fecha y Hora de Compromiso de Terminado.
 - Status
	
#### 	Caso 9:
		El campo Status de cada tarea debera tener minimo las siguientes posibilidades:
			-En Espera (Nunca comenzada)
			-En Proceso (Comenzada almenos una vez)
			-En Pausa (No trabajandose actualmente, pero ya iniciada anteriormente)
			-Terminada.
			-Cancelada (No se realizara mas)
		
#### 	Caso 10:
		Cada tarea podra ser relacionada muchos-a-muchos con 3 tipos de registro:
			-Usuarios (Obligatorio con condiciones): 
				*SI tipo = TAREA:
					El creador de la tarea es la unica relacion minima necesaria para la tarea, pudiendo agregar mas usuarios libremente.
				*SI tipo = MEJORA o tipo = FIX:
					La relacion puede quedar vacia, hasta el momento en que se cambie el Status = En Proceso, en cuyo caso debera tener almenos un Usuario agregado.

			-Etiquetas (Opcional):
				La creacion y asignacion de Etiquetas es libre e ilimitada, por lo que el catalogo de etiquetas debera estar abierto a registros nuevos y estar indexado en base al Texto de la etiqueta.
			
			-Proyectos (Opcional):
				Cualquier tarea puede o no tener uno o mas Proyectos relacionados.

#### 	Caso 11:
			Debera desarrollarse un modulo (de aqui en adelante MODULO DE PROYECTOS) para el registro de Proyectos, que permita crearlos, editarlos, borrarlos y consultarlos.

#### 	Caso 12:



