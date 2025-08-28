# Formato de Especificación Personalizado

## Resumen
Este documento define el formato y estructura de especificación personalizada para proyectos de desarrollo de software, diseñado para trabajar con el flujo de trabajo personalizado mejorado que soporta arquitecturas tanto de monolito como de microservicios.

## Estructura de Directorios
```
aidlc-docs/
├── plans/              # Todos los documentos de planificación (requisitos, historias, diseño, generación de código, unidad de trabajo)
├── requirements/       # Documentos de requisitos detallados  
├── design-artifacts/   # Documentos de diseño técnico, decisiones arquitectónicas y definiciones de servicios
├── story-artifacts/    # Historias de usuario, personas y unidades de trabajo
├── research/           # Notas de investigación e indagación
└── aidlc-state.md      # Archivo maestro de seguimiento de estado con casillas de verificación de fases
└── audit.md            # registrar aprobaciones de los usuarios con marca de tiempo para cada fase AI-DLC
```

## Tipos de Documentos

### Planes (`aidlc-docs/plans/`)
- **Planificación de Requisitos**: requirement-elaboration-plan.md
- **Planificación de Historias**: story-generation-plan.md
- **Planificación de Diseño**: design-generation-plan.md (monolito) o unit-of-work-plan.md (microservicios)
- **Planificación de Generación de Código**: code-generation-plan.md (monolito) o {nombre-unidad}-code-generation-plan.md (microservicios)
- **Planificación de Diseño de Unidad**: {nombre-unidad}-design-plan.md (solo microservicios)

### Requisitos (`aidlc-docs/requirements/`)
- Requisitos funcionales y no funcionales
- Criterios de aceptación en formato EARS
- Restricciones técnicas y dependencias

### Artefactos de Diseño (`aidlc-docs/design-artifacts/`)
- **Decisiones Arquitectónicas**: architectural-decisions.md (registra la elección monolito vs microservicios)
- **Artefactos de Monolito**:
  - design.md, domain-model.md, api-specification.yaml
  - component-diagram.md, component-dependency-matrix.md
- **Artefactos de Microservicios**:
  - unit-of-work.md, unit-of-work-dependency.md, unit-of-work-story-map.md
  - {nombre-unidad}-design.md, {nombre-unidad}-domain-model.md, {nombre-unidad}-api-specification.yaml
  - {nombre-unidad}-component-diagram.md, {nombre-unidad}-data-model.md

### Artefactos de Historias (`aidlc-docs/story-artifacts/`)
- **Historias de Usuario**: Requisitos individuales enfocados en el usuario
- **Personas**: Arquetipos y características de usuarios  
- **Unidades de Trabajo**: Colecciones agrupadas de historias relacionadas que forman incrementos lógicos de desarrollo

### Investigación (`aidlc-docs/research/`)
- Hallazgos de investigación técnica
- Pruebas de concepto y experimentos
- Análisis de dependencias externas e integraciones

### aidlc-state.md
- Rastreador maestro de estado AI-DLC con casillas de verificación de fases
- Se actualiza dinámicamente basado en la elección arquitectónica (monolito vs microservicios)
- Usado por Kiro para determinar la fase actual y próximos pasos
- Contiene sección "Estado Actual" para continuidad de sesión

### audit.md
- Rastro de auditoría de todos los prompts de aprobación y respuestas del usuario
- Registra marcas de tiempo para cada interacción
- Mantiene registro cronológico de puntos de decisión
- Incluye contexto de fase y estado de aprobación para cada entrada

## Convención de Nomenclatura de Archivos
Usar kebab-case para todos los nombres de archivos:

### Archivos Principales
- requirement-elaboration-plan.md
- story-generation-plan.md
- requirements.md
- stories.md, personas.md, units-of-work.md
- architectural-decisions.md

### Archivos Específicos de Monolito
- design-generation-plan.md
- code-generation-plan.md
- design.md, domain-model.md, api-specification.yaml
- component-diagram.md, component-dependency-matrix.md

### Archivos Específicos de Microservicios
- unit-of-work-plan.md
- unit-of-work.md, unit-of-work-dependency.md, unit-of-work-story-map.md
- {nombre-unidad}-design-plan.md
- {nombre-unidad}-code-generation-plan.md
- {nombre-unidad}-design.md, {nombre-unidad}-domain-model.md
- {nombre-unidad}-api-specification.yaml, {nombre-unidad}-component-diagram.md
- {nombre-unidad}-data-model.md

## Integración del Flujo de Trabajo
Este formato de especificación se integra con las fases del flujo de trabajo personalizado mejorado:

### Fases Principales (1-4)
1. **Evaluación de Requisitos**: Crear o actualizar requirements.md
2. **Planificación de Historias**: Crear story-generation-plan.md  
3. **Desarrollo de Historias**: Generar stories.md, personas.md, units-of-work.md
4. **Decisión de Arquitectura**: Crear architectural-decisions.md y actualizar aidlc-state.md

### Ruta Monolito (5-8)
5. **Planificación de Diseño**: Crear design-generation-plan.md
6. **Generación de Diseño**: Crear artefactos de diseño (design.md, domain-model.md, etc.)
7. **Planificación de Generación de Código**: Crear code-generation-plan.md
8. **Generación Iterativa de Código**: Generar código en fases ordenadas por dependencias

### Ruta Microservicios (5-8)
5. **Planificación de Unidades de Trabajo**: Crear unit-of-work-plan.md
6. **Generación de Unidades de Trabajo**: Crear artefactos de descomposición de unidades de trabajo (unit-of-work.md, unit-of-work-dependency.md, unit-of-work-story-map.md)
7. **Diseño y Desarrollo por Unidad**: Repetir para cada unidad de trabajo (componentes frontend y servicios backend)
8. **Integración del Sistema**: Orquestar e integrar todas las unidades de trabajo