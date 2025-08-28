# Pasos de Fase 1: Evaluación de Requisitos

**Asumir el rol** de propietario de producto

**Fase Universal**: Funciona con cualquier entrada - declaraciones de intención, documentos existentes, o contenido mixto

1. **Evaluar Requisitos Actuales**: Analizar lo que el usuario haya proporcionado:
   - Declaraciones de intención o descripciones
   - Documentos de requisitos existentes (buscar en espacio de trabajo si se menciona)
   - Contenido pegado o referencias de archivos
   - Convertir cualquier documento no-markdown a formato markdown

2. **Verificación Intuitiva de Completitud**: Usar inteligencia de Kiro para evaluar si los requisitos son suficientes:
   - **Si son suficientes**: "Los requisitos se ven completos, listo para proceder a historias"
   - **Si son insuficientes**: Identificar brechas específicas y generar preguntas dirigidas

3. **Hacer Preguntas Aclaratorias** (solo si es necesario):
   - Crear `aidlc-docs/requirements/preguntas-verificacion-requisitos.md` con 3-7 preguntas enfocadas sobre áreas faltantes o poco claras usando formato de etiqueta [Respuesta]:
   - Enfocarse en requisitos funcionales, requisitos no funcionales, y escenarios de usuario
   - Solicitar al usuario llenar todas las etiquetas [Respuesta]: directamente en el documento de preguntas
   - Esperar respuestas del usuario en el documento
   - **Obligatorio** seguir haciendo preguntas hasta estar satisfecho con los requisitos o hasta que el usuario pida explícitamente proceder a la siguiente fase.

4. **Generar/Actualizar Documento de Requisitos**:
   - Crear o actualizar `aidlc-docs/requirements/requisitos.md`
   - Incluir tanto requisitos funcionales como no funcionales
   - Incorporar respuestas del usuario a preguntas aclaratorias
   - Proporcionar resumen breve de requisitos clave

5. **Registrar y Proceder**:
   - Registrar prompt de aprobación con marca de tiempo en `aidlc-docs/audit.md`
   - Esperar aprobación explícita del usuario antes de proceder
   - Registrar respuesta de aprobación con marca de tiempo
   - Actualizar Fase 1 completa en aidlc-state.md