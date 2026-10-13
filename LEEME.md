# Arduino Lab Kids — edición ampliada (60 proyectos)

## Abrir
1. Descomprimir el ZIP en una carpeta.
2. Abrir `index.html` con Chrome, Firefox o Edge. No hace falta un servidor.
3. Seleccionar un proyecto y recorrer: Proyecto → Conexiones → Código → Simular → Entender → Modificar → Chequear.
4. Guardar las versiones y exportar regularmente el progreso mediante **Exportar mi avance**. El progreso por defecto está en este navegador; no se sincroniza automáticamente.

## Catálogo
- 10 proyectos originales
- 10 motores paso a paso con controlador A4988
- 10 prácticas de lógica para motores piezoeléctricos reales (ejercicios con LED; NO se simula ni se acciona directamente el motor real)
- 10 luces
- 10 sensores
- 5 sonidos
- 5 juegos

Total: **60 proyectos** con componentes, pasos, códigos y 8 desafíos por proyecto (los originales mantienen sus retos previos).

## Simuladores gratuitos
- Wokwi (acceso rápido, desde el navegador): https://wokwi.com/projects/new/arduino-uno
- Wokwi: componentes simulables: https://docs.wokwi.com/getting-started/supported-hardware
- Tinkercad Circuits (entorno muy visual; podría solicitar iniciar sesión): https://www.tinkercad.com/circuits
- Tutorial Tinkercad: https://www.tinkercad.com/learn/circuits

Para los 20 ejercicios de motores hay carpetas `wokwi/<id>/` con `sketch.ino` y `diagram.json`. En Wokwi abrí un nuevo proyecto Arduino UNO y COPIÁ el contenido de ambos archivos a sus pestañas equivalentes. Son plantillas de simulación, no archivos de circuito físico certificados.

Para los 10 proyectos paso a paso, `diagram.json` incluye el **A4988 + motor bipolar**, y los sensores/pulsadores del proyecto cuando Wokwi dispone del componente. Wokwi simula digitalmente, no calcula la corriente del driver. En montaje físico son obligatorios **fuente de motor independiente adecuada**, **condensador en VMOT** y **ajuste del límite de corriente** del A4988 por parte de un adulto competente. NUNCA conectar un motor de este tipo directamente al UNO, ni conectar/desconectar bobinas con el driver energizado.

Para los 10 proyectos piezoeléctricos, el `diagram.json` **simula un LED de prueba**, NO un motor piezoeléctrico. Los sketches dejan inhabilitada la salida de control externo por defecto (`CONTROLADOR_VERIFICADO = false`). Si se quiere controlar un motor físico, es necesario un controlador homologado para su motor y una interfaz digital documentada compatible; el código de ejemplo debe adaptarse y validarse antes de conectarlo. Un zumbador piezoeléctrico es otra cosa: los proyectos de Sonido usan zumbadores y sí son accesibles para principiantes.

## Código y comprobación
Los 60 sketches `.ino` están en `projects/`. La pestaña **Chequear** realiza verificaciones educativas de texto (llaves, paréntesis, algunas instrucciones), **NO** compila realmente ni detecta todos los errores. La prueba definitiva es compilar/subir en Arduino IDE con la placa correcta o ejecutar una simulación compatible en Wokwi.

## Guardado
El inventario, el progreso de desafíos, los tutoriales marcados y las versiones de código se guardan en el navegador mediante `localStorage`. **Exportar mi avance** guarda un JSON para respaldo; **Recuperar avance** lo importa en otro equipo. Si limpiás datos del navegador sin exportarlo, se pierde.

## Cómo aprender sin copiar a ciegas
Animá al alumno a predecir qué pasará, dibujar conexiones, ejecutar, explicar por qué funciona y recién entonces modificar un valor. Empezar por las luces, seguir por botones, sensores y sonidos, después motores paso a paso y finalmente lógica de control piezoeléctrico, siempre con acompañamiento adulto al cablear motores.

Proyecto educativo; verificar pinouts y especificaciones de cada componente real antes de conectar electricidad.