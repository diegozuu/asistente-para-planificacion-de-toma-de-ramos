# Prototipo 2 - Simulador Institucional Duoc UC 

Esta versión toma la idea del primer prototipo y la lleva al siguiente nivel, creando un simulador interactivo de cómo funcionaría este servicio integrado directamente en el portal de **Duoc UC**.

---

### Principales mejoras respecto al Prototipo 1:

1. **Interfaz simulada de la institución (HTML/CSS):**
   * A diferencia del primer prototipo, aquí se integró una pantalla web adaptada con los colores corporativos (negro y amarillo) y los logos de Duoc UC para simular el portal institucional.

2. **Rol y mentalidad de la IA:**
   * Se configuró el prompt del sistema para que el modelo asuma explícitamente el rol de un **Asistente Virtual Duoc UC**, respondiendo con un tono institucional, amable y enfocado.
   * <img width="1335" height="88" alt="image" src="https://github.com/user-attachments/assets/f92be5da-e2e1-4330-9516-b36f10dcbed1" />


3. **Horarios en tablas organizadas:**
   * La IA ya no responde con texto simple. Ahora está programada para generar obligatoriamente una **tabla estructurada con los bloques de horario, días y secciones**.
   * <img width="1024" height="500" alt="image" src="https://github.com/user-attachments/assets/c3280bf0-4061-4e9f-8746-acb2fa506ec4" />


5. **Estructura mejorada para lectura de PDFs:**
   * Se cambió el formato en el cual se analizan los PDF, añadiendo una estructura que permite identificar los archivos de forma ordenada usando la siguente estructura:  
     `"PalabraClave": "NombreExactoDelArchivo.pdf"`
