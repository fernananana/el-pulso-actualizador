# Actualizador independiente de El pulso del canal

Este repositorio contiene únicamente el programador de una actualización horaria de Wowtogo. No contiene métricas, claves de Google, permisos de renovación, datos del canal ni el código privado que calcula los Consejos.

La tarea usa un equipo estándar gratuito de GitHub Actions. Cada ejecución demuestra su identidad con una firma temporal de GitHub; no tiene secretos guardados. Wowtogo comprueba el repositorio, su propietario, la rama principal, el archivo de tarea y la firma antes de admitir la petición. Una copia de este repositorio no queda autorizada.

La lectura y los Consejos los calcula el mismo servicio privado existente. No se cambia su método, los informes solicitados ni el acceso de solo lectura de YouTube. El equipo de GitHub únicamente activa la lectura y comprueba que las fechas de datos y Consejos coinciden; no recibe los informes privados.

La lectura se programa cada hora en el minuto 17. Se evita el inicio de la hora porque GitHub advierte de mayor carga en ese momento. La tarea reintenta los fallos transitorios sin borrar la lectura anterior. GitHub puede retrasar o suspender ejecuciones durante incidencias de su plataforma; el panel muestra la antigüedad de la lectura.

Una tarea mensual mantiene un registro técnico de actividad en este repositorio para que la programación no quede inactiva por falta de cambios. Ese registro contiene únicamente una fecha de mantenimiento, sin métricas del canal.

Solo se usan equipos estándar, sin servicios de IA, equipos ampliados, almacenamiento de artefactos ni cachés de pago. Documentación: https://docs.github.com/en/billing/concepts/product-billing/github-actions
