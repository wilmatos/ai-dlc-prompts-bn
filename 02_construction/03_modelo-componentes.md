# 03 - Modelo de Componentes

## Definición de Rol

Eres un ingeniero de software experimentado. Antes de comenzar la tarea mencionada a continuación, realiza la planificación y escribe tus pasos en el archivo `design/component_model_plan.md` con checkboxes contra cada paso del plan.

## Requisitos de Auditoría

**CRÍTICO**: Actualizar archivos de auditoría después de cada acción:
1. **Seguimiento de Estado**: Actualizar checkboxes en `audit/estado-aidlc.md`
2. **Registro de Actividad**: Agregar entrada a `audit/registro-actividad.md`

**REGISTRO INICIAL**: Marcar "2.1 Modelo de Componentes - Planificación Iniciada"

## Proceso de Ejecución

### Paso 1: Planificación

Escribe tus pasos en el archivo `design/component_model_plan.md` con checkboxes contra cada paso del plan.

**REGISTRO**: Marcar "2.2 Modelo de Componentes - Plan Creado" al completar el plan

### Paso 2: Clarificaciones

Si algún paso necesita clarificación, agrégalo al paso para interactuar conmigo y obtener confirmación. No tomes decisiones críticas por tu cuenta.

#### Formato de Clarificaciones
```markdown
## Preguntas de Clarificación

**Pregunta 1**: [Descripción sobre arquitectura de componentes]
[Respuesta]: 

**Pregunta 2**: [Descripción sobre patrones de diseño]
[Respuesta]: 

**Pregunta 3**: [Descripción sobre tecnologías específicas]
[Respuesta]: 
```

### Paso 3: Aprobación

Una vez que produzcas el plan, solicita mi revisión y aprobación.

**REGISTRO**: Marcar "2.3 Modelo de Componentes - Plan Aprobado" tras aprobación del usuario

### Paso 4: Ejecución

Después de mi aprobación, ejecuta el mismo plan paso a paso. Una vez que termines cada paso, marca los checkboxes como completados en el plan.

**REGISTRO**: Marcar "2.4 Modelo de Componentes - Modelo Generado"

## Plantilla de Entrada

**Tu Tarea**: Referir a las historias de usuario en el archivo de unidad específica. Diseñar el modelo de componentes para implementar todas las historias de usuario.

```markdown
**Archivo de Unidad**: [INSERTAR_REFERENCIA_ARCHIVO_UNIDAD]

**Patrones Arquitectónicos Preferidos**: [INSERTAR_PATRONES_ARQUITECTONICOS]

**Restricciones Tecnológicas**: [INSERTAR_RESTRICCIONES_TECNOLOGICAS]

**Requisitos No Funcionales**: [INSERTAR_REQUISITOS_NO_FUNCIONALES]

**Integraciones Externas**: [INSERTAR_INTEGRACIONES_EXTERNAS]
```

## Contenido del Modelo

Este modelo debe contener:
- **Componentes**: Todos los componentes del sistema
- **Atributos**: Propiedades de cada componente
- **Comportamientos**: Métodos y funcionalidades
- **Interacciones**: Cómo los componentes interactúan para implementar las historias de usuario

**IMPORTANTE**: No generar código aún. Solo escribir el modelo de componentes en un archivo md separado en la carpeta `/design`.

## Archivos de Salida Esperados

1. **design/component_model_plan.md** - Plan de diseño con checkboxes
2. **design/component_model.md** - Modelo de componentes detallado

## Formato del Modelo de Componentes

```markdown
# Modelo de Componentes - [Nombre de la Unidad]

## Visión General de la Arquitectura
[Descripción general del enfoque arquitectónico]

## Componentes del Sistema

### Componente: [Nombre del Componente]

#### Responsabilidades
- [Responsabilidad 1]
- [Responsabilidad 2]

#### Atributos
- **[nombre_atributo]**: [tipo] - [descripción]
- **[nombre_atributo]**: [tipo] - [descripción]

#### Comportamientos/Métodos
- **[nombre_metodo]([parámetros])**: [descripción y valor de retorno]
- **[nombre_metodo]([parámetros])**: [descripción y valor de retorno]

#### Dependencias
- [Componente dependiente 1]
- [Componente dependiente 2]

## Interacciones entre Componentes

### Flujo: [Nombre del Flujo de Historia de Usuario]
1. [Componente A] → [Componente B]: [descripción de la interacción]
2. [Componente B] → [Componente C]: [descripción de la interacción]
3. [Resultado final]

## Patrones de Diseño Aplicados
- **[Patrón 1]**: [Justificación y aplicación]
- **[Patrón 2]**: [Justificación y aplicación]

## Consideraciones Técnicas
- **Escalabilidad**: [Consideraciones de escalabilidad]
- **Rendimiento**: [Consideraciones de rendimiento]
- **Seguridad**: [Consideraciones de seguridad]
- **Mantenibilidad**: [Consideraciones de mantenibilidad]
```

## Instrucciones de Uso

### Para Continuar desde Unidades Definidas
1. Seleccionar archivo específico `design/unit_[nombre].md`
2. Ejecutar prompt: `@03_modelo-componentes`
3. Revisar y aprobar plan de diseño
4. Confirmar ejecución

### Para Usar Historias de Unidad Externa
1. Especificar ubicación de archivo de unidad existente
2. Verificar que contenga historias de usuario y criterios de aceptación
3. Continuar con proceso normal

### Para Múltiples Unidades
1. Ejecutar prompt por cada unidad por separado
2. Mantener consistencia en patrones arquitectónicos
3. Documentar dependencias entre modelos de componentes

## Validación de Completitud

Antes de marcar como completo, verificar:
- [ ] Todas las historias de usuario están cubiertas por componentes
- [ ] Interacciones entre componentes están claramente definidas
- [ ] Atributos y comportamientos son específicos y completos
- [ ] Patrones de diseño están justificados
- [ ] Consideraciones no funcionales están incluidas
- [ ] Plan ejecutado completamente con checkboxes marcados
- [ ] Archivos de auditoría actualizados

## Ejemplo de Uso

```bash
# Después de definir unidades
@03_modelo-componentes

# Responder cuando se solicite:
# "Archivo de Unidad: design/unit_authentication.md"
# "Patrones Arquitectónicos Preferidos: MVC, Repository Pattern"
# "Restricciones Tecnológicas: Python, PostgreSQL"
```