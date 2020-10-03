#### Universidad Nacional de Colombia
### Arquitectura de Software
## Laboratorio 3

- Julian David Acosta
- Luis Ferney Sandoval
- Juan Camilo Vargas

### 1. Soporte visual de la ejecución de las peticiones sobre la API-GraphQL, y sus acciones evidenciadas en la base de datos.

A continuación se encuentran el soporte visual de cada una de las peticiones y la evidencia de su acción en la base datos, en los casos pertinentes.
Estado inicial de la base de datos:
![01](img/Lab3_01.png)

#### Crear una categoria:

```
mutation {
  createCategory(category: {
    name: "Categoría A",
    description: "Descripción - Categoría A"
  }) {
    name
  }
}
```
Ejecución de la petición:
![02](img/Lab3_02.png)

Base de datos luego de realizar la petición:
![03](img/Lab3_03.png)

#### Actualizar una categoria:

```
mutation {
  updateCategory(id: 10, category: {
    name: "Categoría A"
    description: "Nueva Descripción - Categoría A"
  }) {
    id
    name
    description
  }
}
```
Ejecución de la petición:
![04](img/Lab3_04.png)

Base de datos luego de realizar la petición:
![05](img/Lab3_05.png)

#### Consultar los nombres de todas las categorías:

```
query {
  allCategories {
    name
  }
}
```
Ejecución de la petición:
![06](img/Lab3_06.png)

#### Consultar el id y nombre de una categoria:

```
query {
  categoryById(id: 10) {
    id
    name
  }
}

```
Ejecución de la petición:
![07](img/Lab3_07.png)

#### Eliminar una categoria:

```
mutation {
  deleteCategory(id: 10)
}

```
Ejecución de la petición:
![08](img/Lab3_08.png)

Base de datos luego de realizar la petición:
![09](img/Lab3_09.png)


