# Flujo de Trabajo de Desarrollo de Software Mejorado - Ruta Microservicios

## Resumen
Este flujo de trabajo continúa desde la Fase 4 (Decisión de Arquitectura) cuando el usuario ha elegido el enfoque MICROSERVICIOS.

## Prerrequisitos
- Las Fases 1-4 del core-workflow.md deben estar completas
- Decisión de arquitectura registrada como MICROSERVICIOS en architectural-decisions.md
- aidlc-state.md ha sido actualizado con fases específicas de microservicios

## Fase 5: Planificación de Unidades de Trabajo
1. Cargar todos los pasos desde `phases/microservices-phase5-unit-planning.md`
2. Ejecutar los pasos cargados desde `phases/microservices-phase5-unit-planning.md`
3. Cargar y aplicar `common/answer-analysis-pattern.md`
4. **Pedir Confirmación y ESPERAR**: Preguntar: "Planificación de unidades de trabajo completa. ¿Estás listo para comenzar con la Generación de Unidades de Trabajo?" - NO PROCEDER hasta que el usuario confirme

## Fase 6: Generación de Unidades de Trabajo
1. Cargar todos los pasos desde `phases/microservices-phase6-unit-generation.md`
2. Ejecutar los pasos cargados desde `phases/microservices-phase6-unit-generation.md`
3. **Pedir Confirmación y ESPERAR**: Preguntar: "Generación de unidades de trabajo completa. ¿Estás listo para comenzar con la Fase de Diseño por Unidad?" - NO PROCEDER hasta que el usuario confirme

## Fase 7: Fase de Diseño por Unidad
**Nota**: Se repite para cada unidad de trabajo

1. Cargar todos los pasos desde `phases/microservices-phase7-unit-design.md`
2. Ejecutar los pasos cargados desde `phases/microservices-phase7-unit-design.md`
3. Para la Fase 7.2 (Planificación de Diseño de Unidad), cargar y aplicar `common/answer-analysis-pattern.md`
4. **Pedir Confirmación y ESPERAR**: Preguntar: "Fase de diseño de unidad completa para [nombre-unidad]. ¿Estás listo para continuar con la Generación de Código por Unidad o seleccionar otra unidad para diseño?" - NO PROCEDER hasta que el usuario confirme

## Fase 8: Generación de Código por Unidad
1. Cargar todos los pasos desde `phases/microservices-phase8-unit-code.md`
2. Ejecutar los pasos cargados desde `phases/microservices-phase8-unit-code.md`
3. Para la Fase 8.1 (Planificación de Código de Unidad), cargar y aplicar `common/answer-analysis-pattern.md`
4. **Pedir Confirmación y ESPERAR**: Preguntar: "Generación de código de unidad completa para [nombre-unidad]. ¿Estás listo para continuar con otra unidad o finalizar la implementación de microservicios?" - NO PROCEDER hasta que el usuario confirme

## CRÍTICO: Aplicación de Casillas de Verificación a Nivel de Plan
**OBLIGATORIO**: Cargar y aplicar todas las reglas desde `common/checkbox-enforcement.md`

## Convención de Nomenclatura de Archivos (Específico de Microservicios)
**Referencia**: Cargar convenciones desde `common/microservices-file-conventions.md`
