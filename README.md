# Prompts AI-DLC (Español)

## Descripción General

Esta colección de prompts implementa el marco AI-DLC original con un enfoque de 2 fases: Inception → Construction. Cada prompt está numerado secuencialmente y diseñado para trabajar con las salidas del prompt anterior.

## Estructura de Directorios

```
├── 01_inception/
│   ├── 01_historias-usuario.md
│   └── 02_definicion-unidades.md
├── 02_construction/
│   ├── 03_modelo-componentes.md
│   ├── 04_generacion-codigo.md
│   ├── 05_arquitectura.md
│   └── 06_construccion-iac-apis.md
├── audit/
│   ├── estado-aidlc-legacy.md
│   └── registro-actividad-legacy.md
└── README.md
```

## Orden de Ejecución

### Fase 1: Inception
1. **@01_historias-usuario** - Crear historias de usuario desde requisitos
2. **@02_definicion-unidades** - Agrupar historias en unidades cohesivas

### Fase 2: Construction
3. **@03_modelo-componentes** - Diseñar modelo de componentes
4. **@04_generacion-codigo** - Generar código basado en componentes
5. **@05_arquitectura** - Crear plan de despliegue en la nube
6. **@06_construccion-iac-apis** - Construir IaC y APIs REST

## Uso de Prompts

### Ejecución Secuencial Completa
```bash
# Comenzar desde el inicio
@01_historias-usuario

# Continuar secuencialmente
@02_definicion-unidades
@03_modelo-componentes
@04_generacion-codigo
@05_arquitectura
@06_construccion-iac-apis
```

### Ejecución Desde Punto Intermedio

#### Si ya tienes historias de usuario:
```bash
# Saltar a definición de unidades
@02_definicion-unidades
# Referencia: user_stories.md (archivo existente)
```

#### Si ya tienes unidades definidas:
```bash
# Saltar a modelo de componentes
@03_modelo-componentes
# Referencia: design/unit_*.md (archivos existentes)
```

#### Si ya tienes modelo de componentes:
```bash
# Saltar a generación de código
@04_generacion-codigo
# Referencia: design/component_model.md (archivo existente)
```

## Plantillas de Entrada

### Para Requisitos (Prompt 01)
```markdown
**Descripción de Requisitos**: [INSERTAR_DESCRIPCION_REQUISITOS]
**Archivos de Referencia**: [INSERTAR_REFERENCIAS_ARCHIVOS]
**Restricciones Específicas**: [INSERTAR_RESTRICCIONES]
```

### Para Tecnologías (Prompt 04-06)
```markdown
**Stack Tecnológico**: [INSERTAR_TECNOLOGIAS]
**Plataforma Objetivo**: [INSERTAR_PLATAFORMA]
**Herramientas IaC**: [INSERTAR_HERRAMIENTAS_IAC]
```

## Manejo de Clarificaciones

Cuando un prompt requiere clarificación:

1. **Buscar sección "Preguntas de Clarificación"** en el archivo de plan generado
2. **Responder en los placeholders [Respuesta]**
3. **Solicitar actualización**: "Actualiza el plan con mis respuestas"

### Ejemplo de Clarificación
```markdown
## Preguntas de Clarificación

**Pregunta 1**: ¿Qué tipo de autenticación prefieres?
[Respuesta]: OAuth 2.0 con JWT tokens

**Pregunta 2**: ¿Cuál es la base de datos preferida?
[Respuesta]: PostgreSQL para datos relacionales
```

## Archivos de Salida por Prompt

### 01_historias-usuario
- `user_stories_plan.md` - Plan de trabajo
- `user_stories.md` - Historias de usuario finales
- `acceptance_criteria.md` - Criterios de aceptación

### 02_definicion-unidades
- `units_plan.md` - Plan de agrupación
- `design/unit_*.md` - Archivos por unidad

### 03_modelo-componentes
- `design/component_model_plan.md` - Plan de diseño
- `design/component_model.md` - Modelo de componentes

### 04_generacion-codigo
- `code_generation_plan.md` - Plan de generación
- `backend/` - Código generado

### 05_arquitectura
- `deployment_plan.md` - Plan de despliegue
- `deployment/` - Archivos IaC
- `validation_report.md` - Reporte de validación

### 06_construccion-iac-apis
- `construction_plan.md` - Plan de construcción
- Archivos específicos según tarea

## Seguimiento de Auditoría

Cada prompt actualiza automáticamente:
- **audit/estado-aidlc-legacy.md**: Progreso de fases y etapas
- **audit/registro-actividad-legacy.md**: Log de todas las acciones

## Mejores Prácticas

### Preparación de Entrada
1. **Definir claramente los requisitos** antes del prompt 01
2. **Preparar archivos de referencia** si existen
3. **Especificar restricciones técnicas** desde el inicio

### Durante la Ejecución
1. **Revisar y aprobar cada plan** antes de la ejecución
2. **Responder todas las clarificaciones** completamente
3. **Validar salidas** antes del siguiente prompt

### Reutilización
1. **Identificar punto de entrada** según archivos existentes
2. **Verificar compatibilidad** de formatos de archivo
3. **Actualizar referencias** en prompts según sea necesario

## Resolución de Problemas

### Archivos Faltantes
Si un prompt no encuentra archivos esperados:
1. Verificar nombres de archivo exactos
2. Confirmar ubicación de directorios
3. Ejecutar prompt anterior si es necesario

### Formato Incompatible
Si archivos existentes tienen formato diferente:
1. Revisar estructura esperada en prompt
2. Adaptar archivos existentes al formato
3. Usar placeholders de entrada personalizados

### Clarificaciones Pendientes
Si hay preguntas sin responder:
1. Localizar archivo de plan correspondiente
2. Completar todos los placeholders [Respuesta]
3. Solicitar actualización del plan

## Ejemplos de Uso

### Proyecto Nuevo Completo
```bash
# 1. Preparar requisitos
echo "Sistema de gestión de inventario..." > requirements.md

# 2. Ejecutar secuencia completa
@01_historias-usuario
# [Revisar y aprobar plan]
@02_definicion-unidades
# [Continuar secuencialmente...]
```

### Proyecto con Historias Existentes
```bash
# 1. Verificar formato de historias existentes
# 2. Comenzar desde unidades
@02_definicion-unidades
# Referencia: user_stories.md (existente)
```

### Proyecto Solo para Arquitectura
```bash
# 1. Preparar archivos de componentes
# 2. Saltar a arquitectura
@05_arquitectura
# Referencia: design/component_model.md (existente)
```
```
