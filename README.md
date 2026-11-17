## Mi trabajo: codelab TODO con ViewModel

### Qué construí
Seguí el codelab para reorganizar una aplicación de tareas
hecha con Kotlin y Jetpack Compose. La aplicación permite
agregar tareas, marcarlas como completadas y eliminarlas.

### Cambios realizados
- Separé el modelo Todo del código de la pantalla.
- Creé TodoRepository para administrar la lista de tareas.
- Agregué TodoUiState para representar el estado de la pantalla.
- Creé TodoViewModel para gestionar las acciones y el estado.
- Conecté la interfaz al ViewModel mediante StateFlow y
  collectAsStateWithLifecycle.
- Usé rememberSaveable para el texto que se está escribiendo.
- Agregué cinco pruebas unitarias del ViewModel.

### Conceptos practicados
Practiqué la separación entre datos, lógica e interfaz,
el uso de ViewModel, StateFlow, estados inmutables y pruebas
unitarias con corrutinas.

Las tareas se mantienen en memoria. El ViewModel permite
conservarlas durante cambios de configuración, pero no
proporciona almacenamiento permanente al cerrar la aplicación.

### Compilación y verificación
Configuré GitHub Actions para ejecutar las pruebas unitarias
y generar un APK de depuración.

La ejecución de GitHub Actions finalizó correctamente:
se ejecutaron las pruebas unitarias y se generó el APK de depuración.

[Ver ejecución y descargar APK](https://github.com/DulceG206/TODOViewModel/actions/runs/44014999761)

### Prueba visual
<img width="1366" height="733" alt="Captura de pantalla (337)" src="https://github.com/user-attachments/assets/0060ca06-9ee5-439d-a942-c680a136c67c" />


### Créditos
Proyecto inicial y codelab:
https://github.com/franzueto/TODOViewModel
