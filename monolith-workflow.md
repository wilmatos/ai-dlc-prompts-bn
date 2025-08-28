# Flujo de Trabajo de Desarrollo de Software Mejorado - Ruta Monolito

## Resumen
Este flujo de trabajo continúa desde la Fase 4 (Decisión de Arquitectura) cuando el usuario ha elegido el enfoque MONOLITO.
Este archivo solo debe ser referenciado cuando `aidlc-docs/design-artifacts/architectural-decisions.md` indique que se eligió MONOLITO.

## Prerrequisitos
- Las Fases 1-4 del core-workflow.md deben estar completas
- Decisión de arquitectura registrada como MONOLITO en architectural-decisions.md
- aidlc-state.md ha sido actualizado con fases específicas de monolito

## Fase 5: Planificación de Diseño (Monolito)
1. Cargar todos los pasos desde `phases/monolith-phase5-design-planning.md`
2. Ejecutar los pasos cargados desde `phases/monolith-phase5-design-planning.md`
3. Cargar y aplicar `common/answer-analysis-pattern.md`
4. **Pedir Confirmación y ESPERAR**: Preguntar: "Planificación de diseño completa. ¿Estás listo para comenzar con la Generación de Diseño?" - NO PROCEDER hasta que el usuario confirme

## Fase 6: Generación de Diseño (Monolito)
1. Cargar todos los pasos desde `phases/monolith-phase6-design-generation.md`
2. Ejecutar los pasos cargados desde `phases/monolith-phase6-design-generation.md`
3. **Pedir Confirmación y ESPERAR**: Preguntar: "Generación de diseño completa. ¿Estás listo para comenzar con la Planificación de Generación de Código?" - NO PROCEDER hasta que el usuario confirme

## Fase 7: Planificación de Generación de Código (Monolito)
1. Cargar todos los pasos desde `phases/monolith-phase7-code-planning.md`
2. Ejecutar los pasos cargados desde `phases/monolith-phase7-code-planning.md`
3. Cargar y aplicar `common/answer-analysis-pattern.md`
4. **Pedir Confirmación y ESPERAR**: Preguntar: "Planificación de generación de código completa. ¿Estás listo para comenzar con la Generación Iterativa de Código?" - NO PROCEDER hasta que el usuario confirme

## Fase 8: Generación Iterativa de Código (Monolito)
1. Cargar todos los pasos desde `phases/monolith-phase8-code-generation.md`
2. Ejecutar los pasos cargados desde `phases/monolith-phase8-code-generation.md`
3. **Pedir Confirmación y ESPERAR**: Preguntar: "Generación iterativa de código completa. ¿Estás listo para finalizar la implementación del monolito?" - NO PROCEDER hasta que el usuario confirme

## CRÍTICO: Aplicación de Casillas de Verificación a Nivel de Plan
**OBLIGATORIO**: Cargar y aplicar todas las reglas desde `common/checkbox-enforcement.md`

## Principios Clave para la Ruta Monolito
**Referencia**: Cargar principios desde `monolith/principles.md`

## Convención de Nomenclatura de Archivos (Específico de Monolito)
**Referencia**: Cargar convenciones desde `common/monolith-file-conventions.md`