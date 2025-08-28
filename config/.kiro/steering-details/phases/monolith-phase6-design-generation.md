# Pasos de Fase 6: Generación de Diseño (Monolito)

1. **Crear Documento de Diseño**: Solo después de aprobación del plan de diseño, generar diseño técnico usando metodología aprobada
2. **ACTUALIZACIÓN OBLIGATORIA DEL PLAN**: Mientras trabajas en la generación de diseño, marcar pasos correspondientes como completos en el archivo del plan de diseño cambiando [] a [x] para mostrar progreso de ejecución
3. **Generar Artefactos de Diseño Principales**:
   - **Modelo de Dominio**: Crear `aidlc-docs/design-artifacts/modelo-dominio.md` con entidades, objetos de valor, y relaciones de dominio
   - **Especificación API**: Crear `aidlc-docs/design-artifacts/especificacion-api.yaml` con especificación OpenAPI/Swagger
   - **Diagrama de Componentes**: Crear `aidlc-docs/design-artifacts/diagrama-componentes.md` con diagramas Mermaid mostrando componentes del sistema
   - **Matriz de Dependencias de Componentes**: Crear `aidlc-docs/design-artifacts/matriz-dependencias-componentes.md` mostrando dependencias entre componentes
4. **Almacenar Diseño Principal**: Guardar documento de diseño completo en `aidlc-docs/design-artifacts/diseño.md`
5. **Incluir Arquitectura**: Cubrir diseño del sistema, modelos de datos, y patrones de integración basados en metodología elegida
6. **Resumir Diseño**: Proporcionar un resumen de los artefactos de diseño al usuario
7. **Registrar Prompt de Aprobación**: Antes de pedir aprobación, registrar el prompt con marca de tiempo en `aidlc-docs/audit.md`
8. **Esperar Aprobación**: Obtener aprobación explícita del usuario antes de proceder
9. **Registrar Respuesta de Aprobación**: Registrar la respuesta de aprobación del usuario con marca de tiempo en `aidlc-docs/audit.md`
10. **Actualizar Progreso**: Marcar Fase 6 completa en aidlc-state.md