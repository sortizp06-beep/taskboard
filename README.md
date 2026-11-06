# Taskboard

Gestor de tareas colaborativo en tiempo real, con varios espacios de trabajo y roles, en la línea de Linear o Trello.

> Estado: en desarrollo. Esta es la estructura inicial del repositorio.

## Qué hará

- Registro e inicio de sesión con JWT y refresh tokens rotativos.
- Espacios de trabajo con roles y permisos.
- Tableros, columnas y tarjetas con orden estable.
- Cambios en tiempo real entre usuarios (WebSockets).
- Registro de auditoría, búsqueda de texto completo, notificaciones por cola e invitaciones con caducidad.

## Estructura

Es un monorepo: un solo repositorio con las dos partes del proyecto.

```text
taskboard/
├── backend/    API REST y WebSockets (NestJS, PostgreSQL, Redis)
├── frontend/   Aplicación web (React, Vite, Tailwind)
├── .gitignore
└── README.md
```

## Tecnologías previstas

- **Backend:** NestJS, TypeScript, PostgreSQL, Prisma, Redis, BullMQ, Socket.IO.
- **Frontend:** React, TypeScript, Vite, Tailwind CSS, TanStack Query.
- **Calidad:** Jest, Supertest, Testcontainers, Playwright.
- **Infraestructura:** Docker, GitHub Actions.
