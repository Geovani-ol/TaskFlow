# TaskFlow – Tablero de tareas colaborativo

## 📝 Descripción
TaskFlow es una aplicación web estilo Trello donde los usuarios pueden:
- Registrarse e iniciar sesión (autenticación con Supabase Auth).
- Crear proyectos y dentro de ellos listas de tareas (columnas estilo Kanban).
- Mover tareas entre columnas mediante drag & drop o botones.
- Comentar en cada tarea (relación uno-a-muchos).
- Ver cambios en tiempo real gracias a suscripciones de Supabase.

## 🛠️ Tecnologías utilizadas
- **Frontend**: Astro + React (islas para interactividad).
- **Estilos**: TailwindCSS.
- **Backend (API adicional)**: FastAPI (para lógica como envío de correos o reportes).
- **Base de datos y autenticación**: Supabase (PostgreSQL + Auth + Realtime).
- **Estado global y llamadas**: React Context + fetch/axios (sin herramientas mágicas).

## 🎯 Propósito del proyecto
Proyecto de aprendizaje para dominar:
- Integración de Astro con React (hidratación parcial).
- Uso de Supabase (autenticación, RLS, suscripciones en tiempo real).
- Creación de una API con FastAPI para procesos del lado del servidor.
- Estado global con Context API y comunicación con APIs externas.
- Implementación de drag & drop en React.

## 📁 Estructura conceptual
- Los usuarios se autentican contra Supabase.
- El frontend se comunica directamente con Supabase para operaciones CRUD y realtime.
- FastAPI actúa como capa de servicios adicionales (reportes, emails, etc.).

## ✅ Características principales
| Área | Funcionalidad |
|------|----------------|
| Autenticación | Registro/login con Supabase Auth |
| Proyectos | Crear y gestionar proyectos |
| Tablero | Listas y tareas con ordenación |
| Comentarios | Comentarios anidados por tarea |
| Tiempo real | Sincronización automática entre usuarios |
| API extra | Reportes de progreso (FastAPI) |

## 📚 Aprendizaje esperado
- Construir una app full-stack real con tecnologías modernas.
- Manejar permisos a nivel de base de datos (Row Level Security).
- Implementar colaboración en tiempo real sin servicios externos pesados.
- Separar responsabilidades: frontend, backend propio y BBDD como servicio.