# EstudiantesApp
Desarrollo de Aplicaciones Moviles

Estudiantes.kt : Este archivo proporciona una descripción de la entidad Estudiantes y su mapeo a la base de datos utilizando la biblioteca Room. Esta información es utilizada por Room para crear y manipular la tabla correspondiente en la base de datos, así como para generar el código necesario para interactuar con los objetos Estudiantes en el código de la aplicación.

EstudiantesDB.kt : Este archivo representa la definición de una base de datos llamada EstudiantesDB utilizando la biblioteca Room, y proporciona métodos para acceder a un objeto EstudiantesDao que permite interactuar con la tabla de estudiantes en la base de datos.

EstudiantesDao.kt :  Este archivo representa un DAO (Objeto de Acceso a Datos) utilizado en el contexto de la biblioteca Room en Android para acceder y manipular datos relacionados con estudiantes en una base de datos. Proporciona métodos para realizar operaciones como obtener todos los estudiantes, insertar un estudiante, actualizar un estudiante, eliminar un estudiante y buscar estudiantes por nombre o apellidos.

Constantes.kt : Este archivo define dos constantes de cadena: OPERACION_INSERT y OPERACION_UPDATE, que tienen los valores NUEVO y EDITAR, respectivamente. Estas constantes se pueden utilizar en otros lugares del código para representar operaciones específicas, como insertar o editar en una aplicación de desarrollo de Android.

EstudiantesApp.kt : Este archivo define la clase EstudiantesApp que hereda de la clase Application de Android. Dentro de la función onCreate(), se crea una instancia de la base de datos EstudiantesDB utilizando la biblioteca Room de Android y se asigna a la variable db. La base de datos se inicializa cuando la aplicación se inicia.

EstudiantesAdapter.kt : Este archivo define un adaptador EstudiantesAdapter para un RecyclerView en Android. El adaptador se utiliza para mostrar una lista de objetos Estudiantes en el RecyclerView. La clase interna ViewHolder se utiliza para representar cada elemento individual de la lista. En el método bindItem(), los datos del objeto Estudiantes se enlazan a las vistas correspondientes en el ViewHolder. Además, se establece un OnClickListener en la vista para navegar a otro fragmento cuando se hace clic en ella.

DeleteDialogFragment.kt :  Este archivo define una clase DeleteDialogFragment que muestra un diálogo de confirmación de eliminación. El diálogo tiene dos botones: "Sí" y "Cancelar". Cuando se hace clic en el botón "Sí", se invoca el método borrarEstudiante() en el objeto listener. Cuando se hace clic en el botón "Cancelar", el diálogo se cierra sin realizar ninguna acción adicional. La interfaz DeleteListener se utiliza para comunicar el evento de borrado desde el diálogo a la clase que lo implementa.

EstudiantesListFragment.kt : Este archivo combina el uso de ViewBinding para acceder a las vistas del layout del fragmento de manera segura, ViewModel para almacenar y gestionar los datos relacionados con la UI, y el patrón de observador (Observer) para mantener actualizada la lista de estudiantes mostrada en el RecyclerView.

FormularioFragment.kt : Este archivo define la clase FormularioFragment, que es un fragmento utilizado para mostrar y editar los datos de un estudiante. El fragmento infla una vista, recibe argumentos, inicializa variables, establece observadores y gestiona la interacción del usuario. También utiliza un ViewModel (MainViewModel) para almacenar y manejar los datos relacionados con el estudiante.

MainViewModel.kt : Este archivo actúa como un ViewModel, lo que significa que se encarga de manejar la lógica de presentación y los datos relacionados con la vista en la capa del ViewModel. Proporciona métodos para realizar operaciones como iniciar, guardar, borrar y buscar estudiantes, así como variables observables para almacenar y acceder a los datos de los estudiantes.

activity_main.xml : Este archivo define la estructura y las características visuales de la actividad principal de la aplicación, lo que incluye la ubicación y apariencia de los elementos de la interfaz de usuario, como botones, campos de texto, imágenes u otros componentes personalizados. Este archivo se utiliza para establecer la apariencia visual de la actividad y proporcionar una estructura visual para que los usuarios interactúen con la aplicación.

fragment_estudiantes_list.xml : Este archivo define la interfaz de usuario (UI) para el fragmento EstudiantesListFragment de la aplicación Android. Este archivo representa la vista del fragmento, que es una parte de la interfaz de usuario de la aplicación. La funcionalidad del archivo es mostrar una lista de estudiantes y proporcionar un campo de búsqueda y un botón para agregar nuevos estudiantes.

fragment_formulario.xml : Este archivo presenta un formulario que permite al usuario ingresar su nombre, apellido, edad y número de teléfono. El formulario consta de varios elementos de interfaz de usuario, como campos de texto (EditText) y botones (Button), que permiten al usuario ingresar y guardar la información proporcionada.
item_list.xml : Este archivo define la interfaz de usuario de un elemento de lista. Proporciona la estructura y la apariencia visual para mostrar un elemento de lista con información de nombre y número de teléfono de la aplicación Android.
