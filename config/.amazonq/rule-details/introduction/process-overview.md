# Resumen del Flujo de Trabajo AI-DLC

## El Flujo de Trabajo:
• **Evaluación de Requisitos** → **Historias** → **Elección de Arquitectura** → **Diseño** → **Código**

## El Rol de Tu Equipo:
• **Colaborar juntos** para responder preguntas en documentos de planificación usando etiquetas [Answer]:
• **Trabajar como equipo** para revisar y aprobar cada fase antes de proceder
• **Decidir colectivamente** sobre el enfoque arquitectónico (monolito vs microservicios)
• **Importante**: Este es un esfuerzo de equipo - involucra a las partes interesadas relevantes para cada fase

## Mi Rol:
```
┌─────────────┐    ┌─────────────────┐    ┌─────────────┐    ┌─────────────────┐
│ Crear Plan  │───▶│ Buscar          │───▶│ Modificar   │───▶│ Implementar     │
│             │    │ Aclaración      │    │ Plan        │    │ Plan            │
└─────────────┘    └─────────────────┘    └─────────────┘    └─────────────────┘
       ▲                                                                 │
       │                                                                 │
       └─────────────────────────────────────────────────────────────────┘
```

## Flujo de Trabajo AI-DLC:
```
    ┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
    │ Declaración de  │    │   Documento de  │    │   Entrada       │
    │ Intención       │    │   Requisitos    │    │   Mixta         │
    │ (Nuevo Proyecto)│    │ (Reqs Existentes)│   │ (Cualquier      │
    └─────────────────┘    └─────────────────┘    │ Formato)        │
            │                      │              └─────────────────┘
            │                      │                     │
            └──────────────────────┼─────────────────────┘
                                   ▼
                         ┌───────────────────┐
                         │   Evaluación de   │
                         │    Requisitos     │
                         │ (Inteligencia Q)  │
                         └───────────────────┘
                                   │
                                   ▼
                         ┌─────────────────┐
                         │  Planificación  │
                         │ de Historias de │
                         │    Usuario      │
                         └─────────────────┘
                                   │
                                   ▼
                         ┌─────────────────┐
                         │   Desarrollo    │
                         │ de Historias de │
                         │    Usuario      │
                         └─────────────────┘
                                   │
                                   ▼
                         ┌─────────────────┐
                         │   Decisión de   │
                         │   Arquitectura  │
                         └─────────────────┘
                                   │
                ┌──── Monolito ────┼─── Microservicios ──┐
                │                  │                     │
                ▼                  │                     ▼
        ┌─────────────────┐        │           ┌─────────────────┐
        │     Diseño      │        │           │ Dividir en      │
        │                 │        │           │ Unidades de     │
        │ Modelo Dominio  │        │           │ Trabajo         │
        │       +         │        │           └─────────────────┘
        │  Componentes    │        │                   │
        └─────────────────┘        │                   ▼
                │                  │          ┌─────────────────┐
                ▼                  │          │ Para Cada Unidad│
        ┌─────────────────┐        │          │                 │
        │     Código      │        │          │ ┌─────────────┐ │
        └─────────────────┘        │          │ │   Diseño    │ │
                │                  │          │ └─────────────┘ │
                ▼                  │          │        ↓        │
        ┌─────────────────┐        │          │ ┌─────────────┐ │
        │   Desplegar     │        │          │ │   Código    │ │
        └─────────────────┘        │          │ └─────────────┘ │
                                   │          │        ↓        │
                                   │          │ ┌─────────────┐ │
                                   │          │ │ Desplegar   │ │
                                   │          │ └─────────────┘ │
                                   │          └─────────────────┘
```