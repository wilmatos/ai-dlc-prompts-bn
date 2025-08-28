# Pasos de Fase 7: Planificación de Generación de Código (Monolito)

1. **Crear Plan de Generación de Código**: Generar un plan completo con lista de verificación de ejecución paso a paso para generación de código basado en matriz de dependencias de componentes. Cada paso y sub-paso debe tener una casilla de verificación [].
2. **Analizar Dependencias**: Usar la matriz de dependencias de componentes para determinar orden óptimo de generación de código
3. **Incluir Preguntas de Generación de Código**: EMBEBER TODAS las preguntas dirigidas directamente en el documento del plan usando formato de etiqueta [Respuesta]: sobre:
   - Estándares de codificación y guías de estilo
   - Estructura de carpetas y organización del proyecto
   - Stack tecnológico incluyendo:
     - Tecnología frontend (si aplica)
     - Tecnología backend (si aplica)
     - Enfoque de gestión de datos estáticos
     - Preferencias de plataforma de despliegue
     - Requisitos de Infraestructura como Código (IaaC)
   - Configuración del entorno de desarrollo
   - Enfoque de pruebas (unitarias, integración, e2e)
   - Estrategia de migración de base de datos
   - Preferencias de construcción y despliegue
   - Estándares de calidad de código
4. **Crear Fases de Generación**: Dividir generación de código en fases lógicas basadas en dependencias:
   - Fase 7.1: Componentes núcleo/fundación (sin dependencias)
   - Fase 7.2: Componentes de lógica de negocio (dependen del núcleo)
   - Fase 7.3: Componentes API/Interfaz (dependen de lógica de negocio)
   - Fase 7.4: Componentes de integración (dependen de APIs)
5. **Almacenar Plan de Código**: Guardar el plan completo de generación de código con preguntas embebidas en directorio `aidlc-docs/plans/` como plan-generacion-codigo.md
6. **Solicitar Entrada del Usuario**: Pedir al usuario llenar todas las etiquetas [Respuesta]: directamente en el documento del plan de generación de código para rastro de auditoría
7. **Recopilar Respuestas**: Esperar que el usuario proporcione respuestas a todas las preguntas usando etiquetas [Respuesta]: en el documento
8. **Registrar Prompt de Aprobación**: Antes de pedir aprobación, registrar el prompt con marca de tiempo en `aidlc-docs/audit.md`
9. **Esperar Aprobación Explícita**: No proceder hasta que el usuario apruebe explícitamente el enfoque de generación de código
10. **Registrar Respuesta de Aprobación**: Registrar la respuesta de aprobación del usuario con marca de tiempo en `aidlc-docs/audit.md`
11. **Actualizar Progreso**: Marcar Fase 7 completa en aidlc-state.md