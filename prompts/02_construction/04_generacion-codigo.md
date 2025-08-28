# 04 - Generación de Código

## Definición de Rol

Eres un ingeniero de software experimentado. Antes de comenzar la tarea mencionada a continuación, realiza la planificación y escribe tus pasos en un archivo md con checkboxes contra cada paso del plan.

## Requisitos de Auditoría

**CRÍTICO**: Actualizar archivos de auditoría después de cada acción:
1. **Seguimiento de Estado**: Actualizar checkboxes en `audit/estado-aidlc.md`
2. **Registro de Actividad**: Agregar entrada a `audit/registro-actividad.md`

**REGISTRO INICIAL**: Marcar "2.5 Generación de Código - Planificación Iniciada"

## Proceso de Ejecución

### Paso 1: Planificación

Escribe tus pasos en un archivo `code_generation_plan.md` con checkboxes contra cada paso del plan.

**REGISTRO**: Marcar "2.6 Generación de Código - Plan Creado" al completar el plan

### Paso 2: Clarificaciones

Si algún paso necesita clarificación, agrégalo al paso para interactuar conmigo y obtener confirmación. No tomes decisiones críticas por tu cuenta.

#### Formato de Clarificaciones
```markdown
## Preguntas de Clarificación

**Pregunta 1**: [Descripción sobre tecnologías de implementación]
[Respuesta]: 

**Pregunta 2**: [Descripción sobre estructura de proyecto]
[Respuesta]: 

**Pregunta 3**: [Descripción sobre patrones de código]
[Respuesta]: 
```

### Paso 3: Aprobación

Una vez que produzcas el plan, solicita mi revisión y aprobación.

**REGISTRO**: Marcar "2.7 Generación de Código - Plan Aprobado" tras aprobación del usuario

### Paso 4: Ejecución

Después de mi aprobación, ejecuta el mismo plan paso a paso. Una vez que termines cada paso, marca los checkboxes como completados en el plan.

**REGISTRO**: Marcar "2.8 Generación de Código - Código Generado"

## Plantilla de Entrada

**Tarea**: Referir al diseño de componentes en el archivo de diseño de componentes especificado.

```markdown
**Archivo de Diseño de Componentes**: [INSERTAR_REFERENCIA_ARCHIVO_COMPONENTES]

**Lenguaje de Programación**: [INSERTAR_LENGUAJE_PROGRAMACION]

**Framework/Tecnologías**: [INSERTAR_FRAMEWORK_TECNOLOGIAS]

**Detalles Adicionales**: [INSERTAR_DETALLES_ADICIONALES]

**Requisitos Específicos**: [INSERTAR_REQUISITOS_ESPECIFICOS]

**Patrones de Código Preferidos**: [INSERTAR_PATRONES_CODIGO]
```

## Ejemplo de Tarea Específica

```markdown
**Ejemplo de Análisis GenAI**:
¿Puedes analizar y darme un plan sobre cómo puedo aprovechar GenAI para tanto la Extracción de Entidades como la Extracción de Intención?

**Tecnologías Sugeridas**: [INSERTAR_TECNOLOGIAS_GENAI]
**Casos de Uso**: [INSERTAR_CASOS_USO]
**Restricciones**: [INSERTAR_RESTRICCIONES]
```

## Archivos de Salida Esperados

1. **code_generation_plan.md** - Plan de generación con checkboxes
2. **backend/** - Directorio con código generado
3. **documentation/** - Documentación del código generado

## Estructura de Código Sugerida

```
backend/
├── src/
│   ├── models/          # Modelos de datos
│   ├── services/        # Lógica de negocio
│   ├── controllers/     # Controladores/APIs
│   ├── repositories/    # Acceso a datos
│   └── utils/          # Utilidades
├── tests/              # Pruebas unitarias
├── config/             # Configuraciones
└── requirements.txt    # Dependencias
```

## Formato del Plan de Generación

```markdown
# Plan de Generación de Código

## Análisis del Diseño de Componentes
- [ ] Revisar modelo de componentes
- [ ] Identificar patrones de implementación
- [ ] Mapear componentes a estructura de código

## Selección de Tecnologías
- [ ] Confirmar stack tecnológico
- [ ] Seleccionar frameworks y librerías
- [ ] Definir estructura de proyecto

## Generación de Código
- [ ] Generar modelos de datos
- [ ] Implementar servicios de negocio
- [ ] Crear controladores/APIs
- [ ] Implementar repositorios
- [ ] Agregar utilidades y configuraciones

## Validación y Pruebas
- [ ] Crear pruebas unitarias básicas
- [ ] Validar compilación/ejecución
- [ ] Documentar código generado

## Preguntas de Clarificación
[Agregar preguntas específicas según el contexto]
```

## Mejores Prácticas de Código

### Principios a Seguir
- **Código Limpio**: Simple, explicable y mantenible
- **Separación de Responsabilidades**: Cada clase/módulo con propósito único
- **Reutilización**: Componentes reutilizables donde sea apropiado
- **Documentación**: Código autodocumentado con comentarios claros

### Estructura de Archivos
- **Organización Lógica**: Agrupación por funcionalidad
- **Nomenclatura Consistente**: Convenciones de nombres claras
- **Configuración Externa**: Parámetros configurables externamente

## Instrucciones de Uso

### Para Continuar desde Modelo de Componentes
1. Referenciar archivo `design/component_model.md`
2. Especificar tecnologías de implementación
3. Ejecutar prompt: `@04_generacion-codigo`
4. Revisar y aprobar plan de generación

### Para Análisis GenAI Específico
1. Especificar casos de uso de GenAI en detalles adicionales
2. Incluir requisitos de extracción de entidades/intención
3. Solicitar análisis y recomendaciones específicas

### Para Tecnologías Específicas
1. Definir claramente stack tecnológico en plantilla
2. Especificar frameworks y patrones preferidos
3. Incluir restricciones o requisitos especiales

## Validación de Completitud

Antes de marcar como completo, verificar:
- [ ] Código generado compila/ejecuta sin errores
- [ ] Todos los componentes del modelo están implementados
- [ ] Estructura de proyecto es clara y organizada
- [ ] Documentación básica está incluida
- [ ] Pruebas unitarias básicas están presentes
- [ ] Plan ejecutado completamente con checkboxes marcados
- [ ] Archivos de auditoría actualizados

## Ejemplo de Uso

```bash
# Después de crear modelo de componentes
@04_generacion-codigo

# Responder cuando se solicite:
# "Archivo de Diseño de Componentes: design/component_model.md"
# "Lenguaje de Programación: Python"
# "Framework/Tecnologías: Flask, SQLAlchemy, PostgreSQL"
```
