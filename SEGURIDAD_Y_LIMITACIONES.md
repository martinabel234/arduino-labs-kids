# Seguridad y limitaciones

- Arduino UNO y LED con resistencias se alimentan desde el USB de 5V; desconectar siempre antes de recablear.
- No manipular corriente de red, fuentes abiertas ni electrónica de alto voltaje con chicos.
- A4988: validar bobinas, fuente VMOT, GND común, capacitor, límite de corriente. La simulación no modela disipación ni corriente.
- Motores piezoeléctricos de movimiento: el elemento piezo puede requerir señales y voltajes especializados. Nunca conectar directo al Arduino; adquirir conjunto motor + controlador compatible. Los 10 proyectos son **prototipos lógicos**, no diseños para excitar el piezomotor.
- El esquema visual de la página es conceptual, con tabla de pines. No usarlo en lugar de la hoja de datos del módulo.
- El chequeador incluido es heurístico, no el compilador oficial. Los ejemplos se han pasado por una revisión sintáctica C++ con cabeceras simuladas, no por Arduino CLI ni por prueba eléctrica.
- Los simuladores son webs de terceros y pueden cambiar su disponibilidad o lista de componentes.