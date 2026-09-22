# Preparar Y en la computadora

Estado: paquete preparado; Y no iniciado. Este paquete no es un relevo ni un checkpoint de trabajo.

1. Materializar CONTINUIDAD-AI en C:/Franco_Bemvelon/CONTINUIDAD-AI. Copiar config.example.json
   a config.local.json en esta carpeta. Configurar claude.executable con el binario nativo
   encontrado en la instalación si PATH no lo resuelve; no copiar la ruta personal de otra máquina.
2. Usar METODO-AI limpio en 0f5fd48ae57752419e9e63faa6b69071df966377. La configuración fija ese SHA; init lo verifica.
   El manifiesto y PROJECT mantienen sus identidades aprobadas. La constitución de este arranque
   es 449a9a05e406cf0c821c044908887f88a0dcc1f1.
3. Verificar origin y estado de work-claude-y y audit-chatgpt-y. Si ya tienen trabajo, no limpiar
   ni reiniciar: informar la discrepancia. Comprobar sólo lectura de los clones auxiliares.
4. Verificar autenticación de Claude con su cuenta y suscripción, y acceso Git del auditor a
   lectura y escritura en audit-chatgpt-y. No publicar una escritura ficticia para probar permisos.
   No agregar permisos globales ni usar bypassPermissions. Revisar reglas efectivas locales si
   contradicen las capacidades de la constitución.
5. El archivo permisos-claude.json se pasa sólo a esta sesión mediante --settings. Habilita edición
   en work, lectura de fuentes y comandos Git con cwd explícito de work. No concede shell libre
   ni acceso de escritura ordinaria al objetivo. Las reglas de archivos no son sandbox de Bash.
   La validación inicial de estos permisos debe hacerse en una carpeta sintética equivalente.
   Si se requieren comandos de pruebas del framework elegido, configurar únicamente esos permisos
   cuando se conozcan; no asumir que un permiso documental elimina un bloqueo del runtime.
6. Conectar las dos fábricas de pestañas y verificar la versión reutilizable en un trabajo sintético
   fuera de Y: fresh/current de ambos roles, texto largo con Unicode/rutas/saltos y recuperación de
   una captura sin reenvío. Reutilizar evidencia ya comprobada cuando corresponda; no repetir la
   batería anterior entera. Preservar IDs, recibos y comparaciones. La variante actual no fue
   ejecutada en esta computadora por el agente que preparó este paquete.
7. Ejecutar check con config.local.json y la ruta runtime. Sólo comprueba rutas, origin y versión.
   Luego usar ARRANQUE_ORQUESTADOR.md cuando corresponda iniciar el trabajo.

No modificar el alcance para resolver un problema de transporte. Si una herramienta está
denegada, conservar el resultado íntegro; no suprimir silenciosamente el control.
No guardar prompts, respuestas, tokens ni logs de sesión en este repositorio.

## Archivos

- config.example.json: rutas y coordenadas; copiar a config.local.json antes de usar.
- permisos-claude.json: permisos por sesión para la etapa inicial.
- ARRANQUE_ORQUESTADOR.md: prompt completo para el orquestador.
