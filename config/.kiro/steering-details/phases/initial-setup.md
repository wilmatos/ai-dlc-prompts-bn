# Pasos de Fase de Configuración Inicial

## Prompt de Continuidad de Sesión
Cuando un usuario regresa para continuar trabajando en un proyecto AI-DLC existente, presenta este prompt:

```markdown
**¡Bienvenido de vuelta! Puedo ver que tienes un proyecto AI-DLC existente en progreso.**

Basado en tu aidlc-state.md, aquí está tu estado actual:
- **Proyecto**: [nombre-proyecto]
- **Fase Actual**: [Fase X: Nombre de Fase]
- **Arquitectura**: [Monolito/Microservicios/Aún no decidido]
- **Último Completado**: [Último paso completado]
- **Siguiente Paso**: [Siguiente paso a trabajar]

**¿En qué te gustaría trabajar hoy?**

A) Continuar donde lo dejaste ([Descripción del siguiente paso])
B) Revisar una fase anterior ([Mostrar fases disponibles])

[Respuesta]: 
```

## Instrucciones para Continuidad de Sesión:
1. **Siempre leer aidlc-state.md primero** al detectar proyecto existente
2. **Analizar estado actual** del archivo de flujo de trabajo para poblar el prompt
3. **Adaptar opciones** basado en elección de arquitectura (ocultar opción C para monolito)
4. **Mostrar pasos específicos siguientes** en lugar de descripciones genéricas
5. **Registrar el prompt de continuidad** en audit.md con marca de tiempo