# Requisitos de Registro de Prompts

- **OBLIGATORIO**: Registrar cada prompt de aprobación con marca de tiempo antes de preguntar al usuario
- **OBLIGATORIO**: Registrar cada respuesta del usuario con marca de tiempo después de recibirla
- Usar formato ISO 8601 para marcas de tiempo (YYYY-MM-DDTHH:MM:SSZ)
- Incluir contexto de fase y estado de aprobación para cada entrada
- Mantener orden cronológico de todas las interacciones
- Usar el siguiente formato para cada entrada:

```markdown
## Fase X: [Nombre de la Fase]
**Marca de Tiempo**: 2025-01-28T14:32:15Z
**Prompt**: "[Texto exacto del prompt preguntado al usuario]"
**Respuesta**: "[Respuesta exacta del usuario]"
**Estado**: [Aprobado/Rechazado/Pendiente]
**Contexto**: [Contexto adicional si es necesario]

---
```