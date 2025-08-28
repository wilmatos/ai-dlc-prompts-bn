# 05 - Arquitectura

## Definición de Rol

Eres un Arquitecto de Nube experimentado. Antes de comenzar la tarea mencionada a continuación, realiza la planificación y escribe tus pasos en un archivo `deployment_plan.md` con checkboxes contra cada paso del plan.

## Requisitos de Auditoría

**CRÍTICO**: Actualizar archivos de auditoría después de cada acción:
1. **Seguimiento de Estado**: Actualizar checkboxes en `audit/estado-aidlc.md`
2. **Registro de Actividad**: Agregar entrada a `audit/registro-actividad.md`

**REGISTRO INICIAL**: Marcar "2.9 Arquitectura - Planificación Iniciada"

## Proceso de Ejecución

### Paso 1: Planificación

Escribe tus pasos en un archivo `deployment_plan.md` con checkboxes contra cada paso del plan.

**REGISTRO**: Marcar "2.10 Arquitectura - Plan Creado" al completar el plan

### Paso 2: Clarificaciones

Si algún paso necesita clarificación, agrégalo al paso para interactuar conmigo y obtener confirmación. No tomes decisiones críticas por tu cuenta.

#### Formato de Clarificaciones
```markdown
## Preguntas de Clarificación

**Pregunta 1**: [Descripción sobre plataforma de nube]
[Respuesta]: 

**Pregunta 2**: [Descripción sobre herramientas IaC]
[Respuesta]: 

**Pregunta 3**: [Descripción sobre requisitos de seguridad]
[Respuesta]: 
```

### Paso 3: Aprobación

Una vez que produzcas el plan, solicita mi revisión y aprobación.

**REGISTRO**: Marcar "2.11 Arquitectura - Plan Aprobado" tras aprobación del usuario

### Paso 4: Ejecución

Después de mi aprobación, ejecuta el mismo plan paso a paso. Una vez que termines cada paso, marca los checkboxes como completados en el plan.

**REGISTRO**: Marcar "2.12 Arquitectura - IaC Generado"

## Plantilla de Entrada

**Tarea**: Referir al modelo de diseño de componentes, unidades, arquitectura de nube y código backend.

```markdown
**Modelo de Diseño de Componentes**: [INSERTAR_REFERENCIA_COMPONENTES]

**Unidades del Sistema**: [INSERTAR_REFERENCIA_UNIDADES]

**Arquitectura de Nube**: [INSERTAR_REFERENCIA_ARQUITECTURA]

**Código Backend**: [INSERTAR_REFERENCIA_BACKEND]

**Infraestructura Objetivo**: [INSERTAR_PLATAFORMA_OBJETIVO]

**Tecnología IaC**: [INSERTAR_TECNOLOGIA_IAC]

**Requisitos de Seguridad**: [INSERTAR_REQUISITOS_SEGURIDAD]

**Requisitos de Escalabilidad**: [INSERTAR_REQUISITOS_ESCALABILIDAD]
```

## Tareas a Completar

### Fase de Planificación
1. **Plan de Despliegue End-to-End**
   - Generar plan completo para despliegue del backend en la plataforma objetivo
   - Usar tecnología IaC especificada (CloudFormation, CDK, Terraform)
   - Documentar todos los prerequisitos para el despliegue

### Fase de Ejecución (Después de Aprobación)
2. **Generación de Código IaC**
   - Seguir mejores prácticas de codificación limpia, simple y explicable
   - Todo el código de salida va en la carpeta `deployment/`
   - Validar que el código generado funciona según lo previsto

3. **Validación y Reporte**
   - Crear plan de validación
   - Generar reporte de validación
   - Revisar reporte de validación y corregir todos los problemas identificados
   - Actualizar reporte de validación

## Archivos de Salida Esperados

1. **deployment_plan.md** - Plan de despliegue con checkboxes
2. **deployment/** - Directorio con archivos IaC
3. **validation_plan.md** - Plan de validación
4. **validation_report.md** - Reporte de validación

## Estructura de Despliegue Sugerida

```
deployment/
├── infrastructure/
│   ├── main.tf (o main.yaml)    # Archivo principal IaC
│   ├── variables.tf             # Variables de configuración
│   ├── outputs.tf               # Salidas del despliegue
│   └── modules/                 # Módulos reutilizables
├── scripts/
│   ├── deploy.sh               # Script de despliegue
│   ├── validate.sh             # Script de validación
│   └── cleanup.sh              # Script de limpieza
├── config/
│   ├── dev.tfvars              # Configuración desarrollo
│   ├── staging.tfvars          # Configuración staging
│   └── prod.tfvars             # Configuración producción
└── docs/
    ├── deployment_guide.md     # Guía de despliegue
    └── troubleshooting.md      # Guía de resolución de problemas
```

## Formato del Plan de Despliegue

```markdown
# Plan de Despliegue - [Nombre del Proyecto]

## Análisis de Requisitos
- [ ] Revisar modelo de componentes
- [ ] Analizar requisitos de infraestructura
- [ ] Identificar dependencias externas

## Diseño de Arquitectura de Nube
- [ ] Definir arquitectura de red
- [ ] Especificar servicios de nube requeridos
- [ ] Diseñar estrategia de seguridad
- [ ] Planificar escalabilidad y alta disponibilidad

## Prerequisitos de Despliegue
- [ ] Configuración de cuentas de nube
- [ ] Permisos y roles requeridos
- [ ] Herramientas de desarrollo necesarias
- [ ] Configuraciones de red

## Generación de IaC
- [ ] Crear archivos de infraestructura principal
- [ ] Implementar módulos reutilizables
- [ ] Configurar variables de entorno
- [ ] Crear scripts de automatización

## Validación y Testing
- [ ] Crear plan de validación
- [ ] Ejecutar pruebas de despliegue
- [ ] Validar funcionalidad end-to-end
- [ ] Documentar resultados

## Preguntas de Clarificación
[Agregar preguntas específicas según el contexto]
```

## Mejores Prácticas IaC

### Principios de Diseño
- **Inmutabilidad**: Infraestructura como código versionado
- **Idempotencia**: Ejecuciones repetibles con mismo resultado
- **Modularidad**: Componentes reutilizables y mantenibles
- **Seguridad**: Principio de menor privilegio

### Organización de Código
- **Separación de Entornos**: Configuraciones por ambiente
- **Versionado**: Control de versiones para todos los archivos
- **Documentación**: Comentarios y documentación clara

## Instrucciones de Uso

### Para Continuar desde Código Backend
1. Referenciar archivos en `backend/` y `design/`
2. Especificar plataforma de nube objetivo
3. Ejecutar prompt: `@05_arquitectura`
4. Revisar y aprobar plan de despliegue

### Para Plataformas Específicas
- **AWS**: Especificar servicios AWS preferidos (EC2, ECS, Lambda, etc.)
- **Azure**: Especificar servicios Azure preferidos
- **GCP**: Especificar servicios GCP preferidos
- **On-Premise**: Especificar tecnologías de contenedores/orquestación

### Para Herramientas IaC Específicas
- **Terraform**: Incluir providers y módulos preferidos
- **CloudFormation**: Especificar templates y stacks
- **CDK**: Especificar lenguaje de programación (TypeScript, Python, etc.)

## Validación de Completitud

Antes de marcar como completo, verificar:
- [ ] Plan de despliegue está completo y aprobado
- [ ] Código IaC está generado y organizado
- [ ] Prerequisitos están documentados
- [ ] Plan de validación está creado
- [ ] Reporte de validación está completo
- [ ] Todos los problemas identificados están resueltos
- [ ] Plan ejecutado completamente con checkboxes marcados
- [ ] Archivos de auditoría actualizados

## Ejemplo de Uso

```bash
# Después de generar código backend
@05_arquitectura

# Responder cuando se solicite:
# "Infraestructura Objetivo: AWS"
# "Tecnología IaC: Terraform"
# "Requisitos de Seguridad: VPC privada, WAF, SSL/TLS"
```
