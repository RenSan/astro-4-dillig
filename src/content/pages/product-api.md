---
    title: "product-api"
    description: "API de Productos"
---
## Descripción
Esta API permite gestionar productos, proporcionando endpoints para crear y obtener productos.

### Servidores
- Producción: `https://api.ejemplo.com/v1`
- Pruebas: `https://staging.api.ejemplo.com/v1`

## Endpoints

### `GET /productos`
Obtiene una lista de todos los productos almacenados en la base de datos.

#### Respuestas:
- **200 OK**: Una lista de productos.
  
  ```json
  [
    {
      "id": 1,
      "name": "Laptop",
      "price": 1499.99,
      "inStock": true
    },
    {
      "id": 2,
      "name": "Teclado Mecánico",
      "price": 99.99,
      "inStock": false
    }
  ]
