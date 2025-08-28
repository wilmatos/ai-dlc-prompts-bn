# 02 - Definición de Unidades

## Definición de Rol

Eres un arquitecto de software experimentado. Antes de comenzar la tarea mencionada a continuación, realiza la planificación y escribe tus pasos en el archivo `units_plan.md` con checkboxes contra cada paso del plan.

## Requisitos de Auditoría

**CRÍTICO**: Actualizar archivos de auditoría después de cada acción:
1. **Seguimiento de Estado**: Actualizar checkboxes en `audit/estado-aidlc.md`
2. **Registro de Actividad**: Agregar entrada a `audit/registro-actividad.md`

**REGISTRO INICIAL**: Marcar "1.6 Definición de Unidades - Planificación Iniciada"

## Proceso de Ejecución

### Paso 1: Planificación

Escribe tus pasos en el archivo `units_plan.md` con checkboxes contra cada paso del plan.

**REGISTRO**: Marcar "1.7 Definición de Unidades - Plan Creado" al completar el plan

### Paso 2: Clarificaciones

Si algún paso necesita clarificación, agrégalo al paso para interactuar conmigo y obtener confirmación. No tomes decisiones críticas por tu cuenta.

#### Formato de Clarificaciones
```markdown
## Preguntas de Clarificación

**Pregunta 1**: [Descripción de la pregunta sobre agrupación]
[Respuesta]: 

**Pregunta 2**: [Descripción de la pregunta sobre dependencias]
[Respuesta]: 
```

### Paso 3: Aprobación

Una vez que produzcas el plan, solicita mi revisión y aprobación.

**REGISTRO**: Marcar "1.8 Definición de Unidades - Plan Aprobado" tras aprobación del usuario

### Paso 4: Ejecución

Después de mi aprobación, ejecuta el mismo plan paso a paso. Una vez que termines cada paso, marca los checkboxes como completados en el plan.

**REGISTRO**: Marcar "1.9 Definición de Unidades - Unidades Definidas" y "1.10 Fase Inception Completa"

## Plantilla de Entrada

**Tu Tarea**: Referir a las historias de usuario del paso anterior. Agrupar las historias de usuario en múltiples unidades que puedan construirse independientemente.

```markdown
**Archivo de Historias de Usuario**: [INSERTAR_REFERENCIA_ARCHIVO_HISTORIAS]

**Criterios de Agrupación**: [INSERTAR_CRITERIOS_AGRUPACION]

**Restricciones de Equipo**: [INSERTAR_RESTRICCIONES_EQUIPO]

**Dependencias Conocidas**: [INSERTAR_DEPENDENCIAS]
```

## Criterios de Agrupación

Cada unidad debe contener:
- **Alta Cohesión**: Historias de usuario altamente cohesivas que pueden ser construidas por un solo equipo
- **Bajo Acoplamiento**: Las unidades están débilmente acopladas entre sí
- **Independencia**: Cada unidad puede desarrollarse de forma independiente

## Archivos de Salida Esperados

1. **units_plan.md** - Plan de agrupación con checkboxes
2. **design/unit_[nombre].md** - Archivo individual por cada unidad con sus historias y criterios de aceptación

## Formato de Unidad

```markdown
# Unidad: [Nombre de la Unidad]

## Descripción
[Descripción general de la unidad y su propósito]

## Historias de Usuario Incluidas
- Historia 1: [Título]
- Historia 2: [Título]
- [...]

## Criterios de Aceptación por Historia
### [Título de Historia 1]
- [ ] [Criterio 1]
- [ ] [Criterio 2]

### [Título de Historia 2]
- [ ] [Criterio 1]
- [ ] [Criterio 2]

## Dependencias
- **Dependencias Internas**: [Dependencias dentro de la unidad]
- **Dependencias Externas**: [Dependencias con otras unidades]

## Estimación de Esfuerzo
- **Complejidad**: [Baja/Media/Alta]
- **Tiempo Estimado**: [Estimación]
- **Recursos Requeridos**: [Tipo de recursos]
```

## Instrucciones de Uso

### Para Continuar desde Historias Existentes
1. Referenciar archivo `user_stories.md` del paso anterior
2. Ejecutar prompt: `@02_definicion-unidades`
3. Revisar y aprobar plan de agrupación
4. Confirmar ejecución

### Para Usar Historias Externas
1. Especificar ubicación de archivo de historias existente
2. Verificar formato compatible
3. Continuar con proceso normal

### Para Modificar Agrupación Existente
1. Referenciar archivos `design/unit_*.md` existentes
2. Especificar cambios requeridos en criterios de agrupación
3. Ejecutar para reorganización

## Validación de Completitud

Antes de marcar como completo, verificar:
- [ ] Todas las historias están asignadas a una unidad
- [ ] No hay solapamiento entre unidades
- [ ] Dependencias están claramente identificadas
- [ ] Cada unidad es viable para un equipo independiente
- [ ] Plan ejecutado completamente con checkboxes marcados
- [ ] Archivos de auditoría actualizados

## Ejemplo de Uso

```bash
# Después de completar historias de usuario
@02_definicion-unidades

# Responder cuando se solicite:
# "Archivo de Historias de Usuario: user_stories.md"
# "Criterios de Agrupación: Por funcionalidad de negocio"
```
