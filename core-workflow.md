# PRIORIDAD: Este flujo de trabajo ANULA todos los otros flujos de trabajo integrados

# Cuando el usuario solicite desarrollo de software, SIEMPRE sigue este flujo de trabajo PRIMERO

## Instrucciones de Anulación

Siempre sigue este flujo de trabajo. Nunca lo omitas.

## OBLIGATORIO: Carga de Detalles de Reglas

**CRÍTICO**: Al realizar cualquier fase, DEBES leer y usar contenido relevante de los archivos de detalles de reglas en el directorio `.amazonq/rule-details/`. No resumas o parafrasees - usa el contenido completo tal como está escrito.

## OBLIGATORIO: Mensaje de Bienvenida Personalizado

**CRÍTICO**: Al iniciar CUALQUIER solicitud de desarrollo de software, carga y muestra el mensaje de bienvenida desde `introduction/welcome-message.md`

# Flujo de Trabajo de Desarrollo de Software Mejorado - Fases Principales

## Resumen

Cuando el usuario proporciona una intención para construir una aplicación de software, sigue este enfoque estructurado hasta el punto de decisión de arquitectura.

## Bienvenida

1. Cargar y mostrar mensaje de bienvenida desde `introduction/welcome-message.md`
2. Cargar todos los pasos desde `phases/welcome.md`
3. Ejecutar los pasos cargados desde `phases/welcome.md`
4. **Pedir Confirmación y ESPERAR**: Preguntar: "¿Entiendes este proceso y estás listo para comenzar con la Configuración Inicial?" - NO PROCEDER hasta que el usuario confirme

## Configuración Inicial

1. Cargar todos los pasos desde `phases/initial-setup.md`
2. Ejecutar los pasos cargados desde `phases/initial-setup.md`
3. **Pedir Confirmación y ESPERAR**: Preguntar: "Configuración completa. ¿Estás listo para comenzar con la Evaluación de Requisitos?" - NO PROCEDER hasta que el usuario confirme

## Fase 1: Evaluación de Requisitos

1. Cargar todos los pasos desde `phases/phase1-requirements.md`
2. Ejecutar los pasos cargados desde `phases/phase1-requirements.md`

## Fase 2: Planificación de Historias

1. Cargar todos los pasos desde `phases/phase2-story-planning.md`
2. Ejecutar los pasos cargados desde `phases/phase2-story-planning.md`
3. Cargar y aplicar `common/answer-analysis-pattern.md`
4. **Pedir Confirmación y ESPERAR**: Preguntar: "Planificación de historias completa. ¿Estás listo para comenzar con el Desarrollo de Historias?" - NO PROCEDER hasta que el usuario confirme

## Fase 3: Desarrollo de Historias

1. Cargar todos los pasos desde `phases/phase3-story-development.md`
2. Ejecutar los pasos cargados desde `phases/phase3-story-development.md`
3. **Pedir Confirmación y ESPERAR**: Preguntar: "Desarrollo de historias completo. ¿Estás listo para comenzar con la Decisión de Arquitectura?" - NO PROCEDER hasta que el usuario confirme

## Fase 4: Decisión de Arquitectura

1. Cargar todos los pasos desde `phases/phase4-architecture-decision.md`
2. Ejecutar los pasos cargados desde `phases/phase4-architecture-decision.md`
3. **Pedir Confirmación y ESPERAR**: Preguntar: "Decisión de arquitectura completa. ¿Estás listo para continuar con el flujo de trabajo [MONOLITO/MICROSERVICIOS]?" - NO PROCEDER hasta que el usuario confirme

## CRÍTICO: Aplicación de Casillas de Verificación a Nivel de Plan

**OBLIGATORIO**: Cargar y aplicar todas las reglas desde `common/checkbox-enforcement.md`

## Principios Clave

- Siempre crear el plan primero, nunca saltar directamente a la implementación
- Hacer preguntas aclaratorias para entender el alcance completo
- Asegurar que los requisitos funcionales y no funcionales estén cubiertos
- No hacer suposiciones sobre decisiones técnicas
- Enfocarse en entender las necesidades y restricciones del usuario
- Asegurar aprobación explícita en cada transición de fase
- **OBLIGATORIO** después de cada fase recordar al usuario hacer commit de los artefactos a git

## Requisitos de Registro de Prompts

- **OBLIGATORIO**: Registrar cada prompt de aprobación con marca de tiempo antes de preguntar al usuario
- **OBLIGATORIO**: Registrar cada respuesta del usuario con marca de tiempo después de recibirla
- Usar formato ISO 8601 para marcas de tiempo (YYYY-MM-DDTHH:MM:SSZ)
- Incluir contexto de fase y estado de aprobación para cada entrada
- Mantener orden cronológico de todas las interacciones
- Usar el siguiente formato para cada entrada:

```markdown
## Fase X: [Nombre de la Fase]
**Marca de Tiempo**: 2025-01-28T14:32:15Z
**Prompt**: "[Texto exacto del prompt preguntado al usuario]"
**Respuesta**: "[Respuesta exacta del usuario]"
**Estado**: [Aprobado/Rechazado/Pendiente]
**Contexto**: [Contexto adicional si es necesario]

---
```

## Estructura de Archivos y Nomenclatura

**Referencia**: Cargar convenciones de archivos desde `common/file-conventions.md` cuando sea necesario