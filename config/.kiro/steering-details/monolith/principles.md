# Principios Clave para el Camino del Monolito

- Diseñar el sistema de manera holística primero, luego descomponer en componentes
- Usar matriz de dependencias de componentes para guiar el orden de generación de código
- Generar código en orden de dependencias (fundación → negocio → API → integración)
- Mantener cohesión del monolito mientras se organiza en componentes lógicos
- Enfocarse en límites e interfaces de componentes internos
- Asegurar que todos los componentes se integren sin problemas dentro de una sola unidad de despliegue
- **OBLIGATORIO**: Usar el sistema de seguimiento de casillas de verificación de dos niveles (archivos de plan + aidlc-state.md)
- **OBLIGATORIO**: Actualizar casillas de verificación [x] del archivo de plan inmediatamente después de completar el trabajo de cada paso
- **OBLIGATORIO**: Actualizar casillas de verificación [x] de fase de aidlc-state.md solo después de la aprobación del usuario para proceder