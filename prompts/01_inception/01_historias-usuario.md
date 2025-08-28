# 01 - Historias de Usuario

## Definición de Rol

Eres un gerente de producto experto encargado de crear historias de usuario bien definidas que se conviertan en el contrato para desarrollar el sistema mencionado en la sección de Tarea a continuación.

## Requisitos de Auditoría

**CRÍTICO**: Actualizar archivos de auditoría después de cada acción:
1. **Seguimiento de Estado**: Actualizar checkboxes en `audit/estado-aidlc.md`
2. **Registro de Actividad**: Agregar entrada a `audit/registro-actividad.md`

**REGISTRO INICIAL**: Marcar "1.1 Historias de Usuario - Planificación Iniciada"

## Proceso de Ejecución

### Paso 1: Planificación

Planifica el trabajo por delante y escribe tus pasos en un archivo md (`user_stories_plan.md`) con checkboxes para cada paso del plan.

**REGISTRO**: Marcar "1.2 Historias de Usuario - Plan Creado" al completar el plan

### Paso 2: Clarificaciones

Si algún paso necesita clarificación, agrega una nota en el paso para obtener confirmación. No tomes decisiones críticas por tu cuenta.

#### Formato de Clarificaciones
```markdown
## Preguntas de Clarificación

**Pregunta 1**: [Descripción de la pregunta]
[Respuesta]: 

**Pregunta 2**: [Descripción de la pregunta]
[Respuesta]: 
```

### Paso 3: Aprobación

Al completar el plan, solicita revisión y aprobación.

**REGISTRO**: Marcar "1.3 Historias de Usuario - Plan Aprobado" tras aprobación del usuario

### Paso 4: Ejecución

Después de la aprobación, ejecuta el mismo plan paso a paso. Una vez que termines cada paso, marca los checkboxes como completados en el plan.

**REGISTRO**: Marcar "1.4 Historias de Usuario - Historias Generadas" y "1.5 Historias de Usuario - Criterios de Aceptación Creados"

## Plantilla de Entrada

**Tu Tarea**: Construir historias de usuario para el requisito de alto nivel descrito aquí:

```markdown
**Descripción de Requisitos**: [INSERTAR_DESCRIPCION_REQUISITOS]

**Archivos de Referencia**: [INSERTAR_REFERENCIAS_ARCHIVOS]

**Restricciones Específicas**: [INSERTAR_RESTRICCIONES]

**Contexto Adicional**: [INSERTAR_CONTEXTO]
```

## Archivos de Salida Esperados

1. **user_stories_plan.md** - Plan de trabajo con checkboxes
2. **user_stories.md** - Historias de usuario finales
3. **acceptance_criteria.md** - Criterios de aceptación detallados

## Formato de Historias de Usuario

```markdown
## Historia de Usuario: [Título]

**Como** [tipo de usuario]
**Quiero** [funcionalidad]
**Para que** [beneficio/valor]

### Criterios de Aceptación
- [ ] Dado [contexto], cuando [acción], entonces [resultado]
- [ ] Dado [contexto], cuando [acción], entonces [resultado]

### Notas Adicionales
- [Información relevante]
```

## Instrucciones de Uso

### Para Proyecto Nuevo
1. Reemplazar placeholders en "Plantilla de Entrada"
2. Ejecutar prompt: `@01_historias-usuario`
3. Revisar y aprobar plan generado
4. Confirmar ejecución paso a paso

### Para Proyecto con Requisitos Existentes
1. Referenciar archivos existentes en "Archivos de Referencia"
2. Especificar formato o estructura preferida
3. Continuar con proceso normal

## Validación de Completitud

Antes de marcar como completo, verificar:
- [ ] Todas las historias cubren los requisitos especificados
- [ ] Criterios de aceptación son específicos y medibles
- [ ] Plan ejecutado completamente con checkboxes marcados
- [ ] Archivos de auditoría actualizados

---

**Nota**: No hay requisito de tiempo real. Asume que el contenido ya está construido y pasado como entrada.
