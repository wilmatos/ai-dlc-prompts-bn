# Pasos de Fase 8: Generación Iterativa de Código (Monolito)

1. **Ejecutar Fases de Generación de Código**: Seguir las fases del plan de generación de código aprobado en orden de dependencias
2. **ACTUALIZACIÓN OBLIGATORIA DEL PLAN**: Para cada paso completado en cualquier fase de generación, marcar el paso correspondiente [x] en plan-generacion-codigo.md inmediatamente después de completar el trabajo
3. **Para Cada Fase de Generación**:
   - Generar código para componentes en fase actual
   - Crear pruebas unitarias correspondientes
   - Crear pruebas de integración donde aplique
   - Actualizar documentación
   - **OBLIGATORIO**: Marcar pasos de fase completos en plan-generacion-codigo.md cambiando [] a [x]
4. **Fase 8.1: Componentes Núcleo/Fundación**:
   - Generar código fundacional (modelos, utilidades, servicios núcleo)
   - Configurar estructura del proyecto y configuración
   - Crear esquemas de base de datos y migraciones
   - Generar operaciones CRUD básicas
   - **OBLIGATORIO**: Actualizar casillas de verificación del plan [x] para cada paso completado
5. **Fase 8.2: Componentes de Lógica de Negocio**:
   - Generar servicios de negocio y lógica de dominio
   - Implementar reglas de negocio y validaciones
   - Crear componentes de capa de servicio
   - **OBLIGATORIO**: Actualizar casillas de verificación del plan [x] para cada paso completado
6. **Fase 8.3: Componentes API/Interfaz**:
   - Generar endpoints de API REST
   - Crear controladores de API y enrutamiento
   - Implementar manejo de solicitudes/respuestas
   - Generar documentación de API
   - **OBLIGATORIO**: Actualizar casillas de verificación del plan [x] para cada paso completado
7. **Fase 8.4: Componentes de Integración**:
   - Generar integraciones de servicios externos
   - Crear middleware y preocupaciones transversales
   - Implementar autenticación y autorización
   - Generar configuraciones de despliegue
   - **OBLIGATORIO**: Actualizar casillas de verificación del plan [x] para cada paso completado
8. **Después de Cada Fase**: 
   - Registrar prompt de aprobación con marca de tiempo en `aidlc-docs/audit.md`
   - Solicitar revisión y aprobación del usuario
   - Registrar respuesta de aprobación con marca de tiempo en `aidlc-docs/audit.md`
   - Actualizar progreso en aidlc-state.md
   - Recordar al usuario hacer commit del código a git
9. **Integración Final**: 
   - Asegurar que todos los componentes funcionen juntos
   - Ejecutar suite completa de pruebas
   - Generar documentación final
   - Marcar Fase 8 completa en aidlc-state.md