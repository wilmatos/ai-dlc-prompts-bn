# Pasos de Fase 5: Planificación de Diseño (Monolito)

1. **Crear Plan de Diseño**: Generar un plan completo con lista de verificación de ejecución paso a paso para metodología y enfoque de diseño de monolito. Cada paso y sub-paso debe tener una casilla de verificación [].
2. **Incluir Todas las Preguntas de Diseño**: EMBEBER TODAS las preguntas dirigidas de diseño directamente en el documento del plan usando formato de etiqueta [Respuesta]: sobre:
   - Patrones de arquitectura (por capas, hexagonal, arquitectura limpia, etc.)
   - Preferencias de stack tecnológico
   - Enfoque de diseño de base de datos
   - Estándares de diseño de API
   - Estrategia de organización de componentes
   - Consideraciones de escalabilidad dentro del monolito
   - Estrategia de pruebas
3. **Presentar Opciones de Diseño**: Incluir diferentes metodologías de diseño de monolito (Diseño Dirigido por Dominio, Arquitectura Limpia, Arquitectura por Capas, etc.) en el documento del plan
4. **Almacenar Plan de Diseño**: Guardar el plan completo de diseño con preguntas embebidas en directorio `aidlc-docs/plans/` como plan-generacion-diseño.md
5. **Solicitar Entrada del Usuario**: Pedir al usuario llenar todas las etiquetas [Respuesta]: directamente en el documento del plan de diseño para rastro de auditoría
6. **Recopilar Respuestas**: Esperar que el usuario proporcione respuestas a todas las preguntas usando etiquetas [Respuesta]: en el documento
7. **Evitar Detalles de Implementación**: Enfocarse en metodología y enfoque, no implementaciones específicas de código
8. **Registrar Prompt de Aprobación**: Antes de pedir aprobación, registrar el prompt con marca de tiempo en `aidlc-docs/audit.md`
9. **Esperar Aprobación Explícita**: No proceder hasta que el usuario apruebe explícitamente el enfoque de diseño
10. **Registrar Respuesta de Aprobación**: Registrar la respuesta de aprobación del usuario con marca de tiempo en `aidlc-docs/audit.md`
11. **Actualizar Progreso**: Marcar Fase 5 completa en aidlc-state.md