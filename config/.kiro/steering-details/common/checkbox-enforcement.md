# CRÍTICO: Aplicación de Casillas de Verificación a Nivel de Plan

## REGLAS OBLIGATORIAS PARA LA EJECUCIÓN DEL PLAN
1. **NUNCA completar ningún trabajo sin actualizar las casillas de verificación del plan**
2. **INMEDIATAMENTE después de completar CUALQUIER paso descrito en un archivo de plan, marcar ese paso [x]**
3. **Esto debe suceder en la MISMA interacción donde se completa el trabajo**
4. **Ejemplo**: Al generar documento de requisitos, marcar "Generar requisitos funcionales" como [x] en requirement-elaboration-plan.md
5. **SIN EXCEPCIONES**: Cada finalización de paso del plan DEBE ser rastreada con actualizaciones de casillas de verificación

## Sistema de Seguimiento de Casillas de Verificación de Dos Niveles
El flujo de trabajo utiliza un sistema de seguimiento de casillas de verificación de dos niveles:

### 1. Seguimiento de Ejecución a Nivel de Plan (Archivos de Plan)
- **Propósito**: Rastrear el progreso detallado de ejecución dentro de cada fase
- **Ubicación**: Archivos de plan individuales (requirement-elaboration-plan.md, story-generation-plan.md, etc.)
- **Cuándo Actualizar**: Marcar pasos [x] al completar el trabajo específico descrito en ese paso
- **OBLIGATORIO**: Actualizar inmediatamente después de completar el trabajo, nunca omitir este paso

### 2. Seguimiento de Progreso a Nivel de Fase (aidlc-state.md)
- **Propósito**: Rastrear el progreso general del flujo de trabajo a través de las fases
- **Ubicación**: aidlc-docs/aidlc-state.md
- **Cuándo Actualizar**: Marcar fases [x] solo cuando toda la fase esté completa y aprobada por el usuario

## Reglas de Actualización Obligatorias
- **Archivos de Plan**: Actualizar casillas de verificación [x] inmediatamente después de completar el trabajo de cada paso
- **aidlc-state.md**: Actualizar casillas de verificación de fase [x] solo después de la aprobación del usuario para proceder
- **Estado Actual**: Siempre actualizar la sección "Estado Actual" en aidlc-state.md después de cualquier progreso
- **Misma Interacción**: Todas las actualizaciones de progreso deben suceder en la MISMA interacción donde se completa el trabajo
- **Nunca Omitir**: Nunca terminar una interacción sin actualizar el seguimiento de progreso