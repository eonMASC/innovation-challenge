# CONVOCATORIA:

EONCORE se complace en convocar a cualquier persona dentro de la empresa (sin contar a los jefes de desarrollo) al Innovation Challenge v1.0, el cual busca promover los valores de competitividad, autoaprendizaje, investigación e innovación en beneficio del crecimiento profesional y laboral de cada uno de los involucrados y por ende de la empresa misma.

El objetivo final será desarrollar un prototipo funcional de sistema web que sirva como base del **"Sistema Interno de Información"**, útil como herramienta diaria de trabajo en las labores de todas a las áreas de la empresa.

---

## Bases:

1. Deberán participar de manera individual y sin asesoría de ningún personal a cargo.
2. Es de carácter obligatorio para el personal de Desarrollo y opcional para el resto de los departamentos.
3. Se dará obligatoriamente 1 hora de horario laboral mínimo, cada uno de los días laborales a partir del día 4 de Noviembre y hasta el Jueves 3 de Diciembre.
4. Las instalaciones de EONCORE están disponibles para el desarrollo de los proyectos las 24 horas de los fines de semana, así como de 6:00 PM a 9:00 AM entre semana.


## Requerimientos Técnicos mínimos:

 1. Tecnologías Requeridas:
   2. **AngularJS 1.4+.** (Recomendado 1.5)
   3. **NodeJS  0.11+.** (Recomendado 4.0+)
   4. Bases de Datos permitidas:
     5. **MySQL / MariaDB**
     6. **MongoDB**
     7. **RethinkDB**
     8. **FireBase** (Solo Database)
   5. **Bootstrap 3+**
   6. **Angular Material**
   7. Repositorio publico en **GitHub**

 2. Tecnologías de valor Extra (Opcionales) :
     1. **Gulp:** Para automatización de la implementación.
     2. **Bower:** Para manejo de dependencias FrontEnd.
     3. **NPM:** Hacer modulo de Node una o mas partes del proyecto.
     4. Captcha Avanzado: Elementos de Autenticación por Audio o Interacción, diferente a Imágenes con caracteres ofuscados. 

## Características del Proyecto (Casos de Uso):

####  Caso 1:
El sistema deberá ser tipo Panel con acceso por autenticación con cuenta de Correo y Contraseña.

####  Caso 2:
Las cuentas de usuario deberán ser almacenadas en BD, la contraseña deberá ser encriptada con algoritmos no reversibles, así como almacenar en bitácora los inicios y cierres de sesión.
  
####  Caso 3:
El sistema requiere Control de Acceso (ACL) con tabla de permisos y asignación por usuario.
  
####  Caso 4:
El panel deberá tener una área de Menú, el cual deberá conformarse de opciones dinámicas almacenadas en BD, que representen a los Módulos registrados/instalados con posibilidad de estar activos o inactivos.

####  Caso 5:
Deberá desarrollarse un modulo (llamado de aquí en adelante **MODULO DE TAREAS**) para el registro de la Bitácora de Tareas, que permita crearlas, editarlas, borrarlas y consultarlas. 

####  Caso 6: 
Cada tarea deberá poderse dar de alta con 3 datos mínimos, 1 capturado por el usuario, que es el Titulo, los otros datos mínimos requeridos tendrán valor por default:

 1. **Titulo** (Obligatorio capturado)
 2. **Fecha y Hora de Creación** (Obligatorio por default): Sera igual a la fecha y hora de creación hasta que el usuario decida alterar este campo y asignar otra fecha-hora de inicio de la tarea.
 3. **Usuario que Creo la Tarea** (Obligatorio = Usuario de la Sesión activa).

####  Caso 7:
Cada tarea deberá ser de 1 solo tipo dentro de los 3 posibles, que son:
 - **PLANIFICADA**.
 - **MEJORA** (Propuesta libre).
 - **CORRECCIÓN** (Corrección de Error).

####  Caso 8:
Cada tarea tendrá mas campos opcionales, que podrán ser agregados en forma de captura/edición ampliada, los cuales son:
 - Descripción.
 - Fecha y Hora de Terminado.
 - Fecha y Hora de Compromiso de Terminado.
 - Status.
  
####  Caso 9:
El campo Status de cada tarea deberá tener mínimo las siguientes posibilidades:
 - **En Espera** (Nunca comenzada).
 - **En Proceso** (Comenzada al menos una vez).
 - **En Pausa** (No trabajándose actualmente, pero ya iniciada anteriormente).
 - **Terminada**.
 - **Cancelada** (No se realizara mas).
    
####  Caso 10:
Cada tarea podrá ser relacionada muchos-a-muchos con 3 tipos de registro:
 - Usuarios (Obligatorio con condiciones): 
   * SI **tipo = PLANIFICADA**: El creador de la tarea es la única relación mínima necesaria para la tarea, pudiendo agregar mas usuarios libremente.
   * SI **tipo = MEJORA o tipo = CORRECCIÓN**: La relación puede quedar vacía, hasta el momento en que se cambie el Status = En Proceso, en cuyo caso deberá tener al menos un Usuario agregado.

 - Etiquetas (Opcional): La creación y asignación de Etiquetas es libre e ilimitada, por lo que el catalogo de etiquetas deberá estar abierto a registros nuevos y estar indexado en base al Texto de la etiqueta.
      
 - Proyectos (Opcional): Cualquier tarea puede o no tener uno o mas Proyectos relacionados.

####  Caso 11:
Deberá desarrollarse un modulo (de aquí en adelante **MODULO DE PROYECTOS**) para el registro de Proyectos, que permita crearlos, editarlos, borrarlos y consultarlos.

####  Caso 12:


## Definición del Ganador y Premiación:

 1. La presentacion y revision final se llevara a cabo el dia Viernes 4 de Diciembre, a las 10:00 hrs. en la sala de juntas de la empresa.

 2. Dispondran de 20 minutos para la presentación en pantalla del sistema desarrollado



