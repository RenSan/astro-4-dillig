---
    title: "order-api"
    description: "API de Órdenes"
---
## Descripción
Esta API permite gestionar órdenes, proporcionando endpoints para crear nuevas órdenes y obtener el listado de órdenes existentes.

### Servidores
- Producción: `https://api.ejemplo.com/v1`
- Pruebas: `https://staging.api.ejemplo.com/v1`

## Endpoints

### `GET /ordenes`
Obtiene una lista de todas las órdenes procesadas en el sistema.

#### Respuestas:
- **200 OK**: Una lista de órdenes.

  ```json
  [
    {
      "id": 101,
      "customer": "Juan Pérez",
      "items": [
        {
          "product": "Laptop",
          "quantity": 1,
          "price": 1499.99
        }
      ],
      "total": 1499.99,
      "status": "Enviado"
    },
    {
      "id": 102,
      "customer": "María López",
      "items": [
        {
          "product": "Teclado Mecánico",
          "quantity": 2,
          "price": 99.99
        }
      ],
      "total": 199.98,
      "status": "Procesando"
    }
  ]
