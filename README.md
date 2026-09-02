# CRM Basic

CRM ligero de una sola página para gestión de clientes, venta de productos digitales y redacción de publicaciones para redes sociales. Todo en `index.html`, sin base de datos: los datos se guardan en `localStorage` del navegador.

## Funcionalidades

**Clientes**
- Alta, edición y borrado de clientes (nombre, email, teléfono, estado).
- Estados: activo, potencial, inactivo, perdido (con badges de color).
- Búsqueda por nombre/email y filtro por estado.
- Panel de estadísticas (total, activos, potenciales, perdidos).

**eCommerce**
- Catálogo de productos digitales (ebooks, cursos, plantillas, servicios) con nombre, descripción y precio.

**Redes Sociales**
- Editor de publicaciones por red (Instagram, Facebook, LinkedIn, TikTok, X) pensado como embudo de tráfico hacia la tienda.

## Stack

- Frontend: HTML/CSS/JS vanilla, sin dependencias, persistencia en `localStorage`.
- Servidor: Express (`server.js`) que sirve los archivos estáticos y hace fallback a `index.html`.

## Uso local

```bash
npm install
npm start
```

La app queda disponible en `http://localhost:3000` (o el puerto de la variable `PORT`).

## Despliegue

Configurado para desplegarse en Railway (u otro proveedor compatible con Node ≥18) usando `npm start` como comando de arranque.
