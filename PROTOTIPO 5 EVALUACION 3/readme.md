# Prototipo 5 logs y dashboard

Este es el quinto prototipo del asistente de horarios para Duoc UC. En las versiones anteriores el sistema solo leía la malla y armaba horarios. Ahora agregué herramientas para medir cómo funciona por dentro, guardar registros de lo que pasa y exigir la malla antes de empezar.

## Qué cambió en este prototipo

* **Nuevo requisito del Agente Analista:** Antes, el primer agente solo buscaba el semestre y la jornada en tu mensaje para pasárselos al siguiente agente. Ahora también revisa si ya subiste la imagen de tu malla al sistema. Si no hay ninguna malla cargada, el agente frena el proceso y te pide subirla en formato JPG o PNG antes de seguir.
* **Medición de tiempos y errores:** El sistema ahora mide cuántos milisegundos tarda cada parte en responder, cuántos tokens gasta y cuántas veces acierta cuando escribes con errores de tipeo.
* **Registros de ejecución:** Cada consulta guarda un código único y anota si hubo avisos o errores. Así puedo ver rápido si falta algún ramo en el Excel o si algo falló.
* **Panel de monitoreo:** Agregué una pestaña nueva con gráficos para ver los tiempos de respuesta, los errores y la precisión del asistente.
* **Seguridad y privacidad:** El sistema revisa que los horarios entregados existan de verdad en el Excel para que la IA no invente secciones.

<img width="676" height="189" alt="image" src="https://github.com/user-attachments/assets/b8e8ccae-53d5-4851-a9f6-a943e442bc4e" />



## Cómo ejecutar y probar el sistema

Para revisar que todo funcione bien, sigue estos pasos:

1. Abre el cuaderno `.ipynb` en Google Colab comprueba tu apy key de Groq y ejecuta todas las celdas en orden hasta que aparezca la interfaz.
2. Sube el archivo Excel con los horarios y la imagen JPG o PNG de una malla en el panel izquierdo.
3. Escribe una consulta en el chat, por ejemplo: *"Paso a 3er semestre en jornada vespertina"*.
4. Abre la pestaña de monitoreo para revisar los gráficos, los tiempos de cada agente y los registros guardados.

<img width="1910" height="815" alt="image" src="https://github.com/user-attachments/assets/21dc1392-06ee-43b2-b140-b8028ef7ea70" />



## Validar con pruebas automáticas

Al final del cuaderno dejé una celda con pruebas automáticas. Al ejecutarla, el sistema simula distintos mensajes con abreviaciones, errores al escribir, cambios de jornada y consultas sin malla. Esto sirve para comprobar que los agentes respondan bien y para actualizar los números del panel de monitoreo.

## Flujo del prototipo 5
<img width="1318" height="666" alt="Gemini_Generated_Image_bco2wkbco2wkbco2" src="https://github.com/user-attachments/assets/ed9c8e5b-4b11-475f-a7d8-680b57d13e87" />
