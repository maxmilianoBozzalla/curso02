⚙️ Explicación de los triggers

El proyecto utiliza distintos triggers de GitHub Actions para ejecutar workflows automáticamente según determinados eventos.

🔹 push

Se activa cuando se realizan cambios en el repositorio y se envían (push) a una rama específica.
Permite validar automáticamente el código ante cada actualización.

🔹 pull_request

Se ejecuta cuando se crea o actualiza un Pull Request hacia una rama (por ejemplo, main).
Se utiliza para verificar que los cambios propuestos cumplen con los requisitos antes de ser integrados.

🔹 issues

Se activa cuando se crea un nuevo issue en el repositorio.
Permite automatizar tareas relacionadas con la gestión de incidencias o solicitudes.

🔹 issue_comment

Se ejecuta cuando se agrega un comentario en un issue o Pull Request.
En este proyecto, se utiliza con una condición para ejecutarse únicamente cuando el comentario pertenece a un Pull Request.

🔹 workflow_dispatch

Permite ejecutar un workflow manualmente desde la interfaz de GitHub.
Admite parámetros de entrada, como en este caso un nivel de alerta seleccionable.

🔹 schedule

Se ejecuta automáticamente en intervalos de tiempo definidos mediante una expresión cron.
Se utiliza para tareas programadas, como procesos periódicos o verificaciones automáticas.
