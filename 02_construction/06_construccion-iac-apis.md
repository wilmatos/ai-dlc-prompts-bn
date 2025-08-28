# 06 - Construcción IaC/APIs REST

## Definición de Rol

Eres un ingeniero de software experimentado. Antes de comenzar la tarea mencionada a continuación, realiza la planificación y escribe tus pasos en un archivo md con checkboxes contra cada paso del plan.

## Requisitos de Auditoría

**CRÍTICO**: Actualizar archivos de auditoría después de cada acción:
1. **Seguimiento de Estado**: Actualizar checkboxes en `audit/estado-aidlc.md`
2. **Registro de Actividad**: Agregar entrada a `audit/registro-actividad.md`

**REGISTRO INICIAL**: Marcar "2.13 Construcción IaC/APIs - Planificación Iniciada"

## Proceso de Ejecución

### Paso 1: Planificación

Escribe tus pasos en un archivo `construction_plan.md` con checkboxes contra cada paso del plan.

**REGISTRO**: Marcar "2.14 Construcción IaC/APIs - Plan Creado" al completar el plan

### Paso 2: Clarificaciones

Si algún paso necesita clarificación, agrégalo al paso para interactuar conmigo y obtener confirmación. No tomes decisiones críticas por tu cuenta.

#### Formato de Clarificaciones
```markdown
## Preguntas de Clarificación

**Pregunta 1**: [Descripción sobre implementación específica]
[Respuesta]: 

**Pregunta 2**: [Descripción sobre tecnologías o frameworks]
[Respuesta]: 

**Pregunta 3**: [Descripción sobre patrones de API]
[Respuesta]: 
```

### Paso 3: Aprobación

Una vez que produzcas el plan, solicita mi revisión y aprobación.

**REGISTRO**: Marcar "2.15 Construcción IaC/APIs - Plan Aprobado" tras aprobación del usuario

### Paso 4: Ejecución

Después de mi aprobación, ejecuta el mismo plan paso a paso. Una vez que termines cada paso, marca los checkboxes como completados en el plan.

**REGISTRO**: Marcar "2.16 Construcción IaC/APIs - Implementación Completa" y "2.17 Fase Construction Completa"

## Plantilla de Entrada

**Tarea**: Proporcionar un placeholder con descripción de qué describir aquí.

```markdown
**Descripción de la Tarea**: [INSERTAR_DESCRIPCION_TAREA_ESPECIFICA]

**Archivos de Referencia**: [INSERTAR_REFERENCIAS_ARCHIVOS]

**Tecnologías Específicas**: [INSERTAR_TECNOLOGIAS_ESPECIFICAS]

**Requisitos de Implementación**: [INSERTAR_REQUISITOS_IMPLEMENTACION]

**Patrones de API Preferidos**: [INSERTAR_PATRONES_API]

**Configuraciones Específicas**: [INSERTAR_CONFIGURACIONES]
```

## Ejemplos de Tareas Específicas

### Ejemplo 1: APIs Flask desde Services.py
```markdown
**Descripción de la Tarea**: Revisar el archivo services.py bajo la carpeta construction/[carpeta]/. Crear APIs Flask de Python para cada uno de los servicios allí.

**Archivos de Referencia**: construction/[carpeta]/services.py
**Tecnologías Específicas**: Python Flask, SQLAlchemy
**Patrones de API Preferidos**: RESTful APIs, JSON responses
```

### Ejemplo 2: Construcción de Microservicios
```markdown
**Descripción de la Tarea**: Implementar microservicios basados en el modelo de componentes usando contenedores Docker.

**Archivos de Referencia**: design/component_model.md, backend/
**Tecnologías Específicas**: Docker, Kubernetes, FastAPI
**Patrones de API Preferidos**: OpenAPI/Swagger, Circuit Breaker
```

### Ejemplo 3: Integración con Servicios de Nube
```markdown
**Descripción de la Tarea**: Integrar las APIs con servicios de AWS (S3, RDS, Lambda) usando el código IaC generado.

**Archivos de Referencia**: deployment/, backend/
**Tecnologías Específicas**: AWS SDK, Boto3, CloudFormation
**Configuraciones Específicas**: IAM roles, VPC configuration
```

## Archivos de Salida Esperados

1. **construction_plan.md** - Plan de construcción con checkboxes
2. **apis/** - Directorio con APIs implementadas
3. **tests/** - Pruebas para las APIs
4. **documentation/** - Documentación de APIs

## Estructura de APIs Sugerida

```
apis/
├── app/
│   ├── __init__.py
│   ├── models/              # Modelos de datos
│   ├── routes/              # Rutas/endpoints de API
│   ├── services/            # Lógica de negocio
│   ├── utils/               # Utilidades
│   └── config.py            # Configuración
├── tests/
│   ├── test_routes.py       # Pruebas de endpoints
│   ├── test_services.py     # Pruebas de servicios
│   └── conftest.py          # Configuración de pruebas
├── requirements.txt         # Dependencias
├── Dockerfile              # Contenedor Docker
├── docker-compose.yml      # Orquestación local
└── README.md               # Documentación
```

## Formato del Plan de Construcción

```markdown
# Plan de Construcción - [Descripción de la Tarea]

## Análisis de Requisitos
- [ ] Revisar archivos de referencia
- [ ] Identificar servicios/componentes a implementar
- [ ] Definir estructura de APIs

## Diseño de APIs
- [ ] Definir endpoints y métodos HTTP
- [ ] Especificar esquemas de request/response
- [ ] Diseñar manejo de errores
- [ ] Planificar autenticación/autorización

## Implementación
- [ ] Crear estructura base del proyecto
- [ ] Implementar modelos de datos
- [ ] Desarrollar lógica de servicios
- [ ] Crear endpoints de API
- [ ] Implementar middleware y utilidades

## Testing y Validación
- [ ] Crear pruebas unitarias
- [ ] Implementar pruebas de integración
- [ ] Validar endpoints con herramientas (Postman, curl)
- [ ] Documentar APIs (Swagger/OpenAPI)

## Despliegue y Configuración
- [ ] Crear archivos de configuración
- [ ] Implementar contenedorización
- [ ] Configurar variables de entorno
- [ ] Documentar proceso de despliegue

## Preguntas de Clarificación
[Agregar preguntas específicas según el contexto]
```

## Mejores Prácticas de APIs

### Diseño RESTful
- **Recursos**: Usar sustantivos para endpoints
- **Métodos HTTP**: GET, POST, PUT, DELETE apropiados
- **Códigos de Estado**: Usar códigos HTTP estándar
- **Versionado**: Implementar versionado de APIs

### Seguridad
- **Autenticación**: JWT, OAuth, API Keys
- **Autorización**: Control de acceso basado en roles
- **Validación**: Validar todas las entradas
- **Rate Limiting**: Limitar frecuencia de requests

### Documentación
- **OpenAPI/Swagger**: Especificación estándar
- **Ejemplos**: Incluir ejemplos de request/response
- **Códigos de Error**: Documentar todos los errores posibles

## Instrucciones de Uso

### Para APIs desde Services.py
1. Especificar ubicación exacta del archivo services.py
2. Definir framework preferido (Flask, FastAPI, Django)
3. Ejecutar prompt: `@06_construccion-iac-apis`

### Para Microservicios
1. Referenciar modelo de componentes y código backend
2. Especificar tecnologías de contenedorización
3. Definir patrones de comunicación entre servicios

### Para Integraciones Específicas
1. Especificar servicios externos a integrar
2. Incluir credenciales y configuraciones necesarias
3. Definir patrones de manejo de errores

## Validación de Completitud

Antes de marcar como completo, verificar:
- [ ] Todas las APIs están implementadas según especificación
- [ ] Pruebas unitarias y de integración pasan
- [ ] Documentación de APIs está completa
- [ ] Configuración de despliegue está lista
- [ ] Manejo de errores está implementado
- [ ] Seguridad básica está configurada
- [ ] Plan ejecutado completamente con checkboxes marcados
- [ ] Archivos de auditoría actualizados

## Ejemplo de Uso

```bash
# Para crear APIs Flask desde services.py
@06_construccion-iac-apis

# Responder cuando se solicite:
# "Descripción de la Tarea: Crear APIs Flask para services.py"
# "Archivos de Referencia: backend/services.py"
# "Tecnologías Específicas: Python Flask, SQLAlchemy, PostgreSQL"
```

## Plantillas de Tareas Comunes

### Tarea: APIs REST desde Servicios
```markdown
**Descripción**: Revisar services.py en [ubicación]. Crear APIs REST para cada servicio.
**Framework**: [Flask/FastAPI/Django]
**Base de Datos**: [PostgreSQL/MySQL/MongoDB]
**Autenticación**: [JWT/OAuth/API Key]
```

### Tarea: Microservicios con Docker
```markdown
**Descripción**: Convertir componentes en microservicios independientes.
**Contenedorización**: Docker + Docker Compose
**Orquestación**: [Kubernetes/Docker Swarm]
**Comunicación**: [REST/gRPC/Message Queue]
```

### Tarea: Integración con Nube
```markdown
**Descripción**: Integrar APIs con servicios de nube específicos.
**Proveedor**: [AWS/Azure/GCP]
**Servicios**: [S3/RDS/Lambda/etc.]
**IaC**: [Terraform/CloudFormation/ARM]
```