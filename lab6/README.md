#### Universidad Nacional de Colombia
### Arquitectura de Software
## Laboratorio 6

- Julian David Acosta
- Luis Ferney Sandoval
- Juan Camilo Vargas

### 1. Despliegue de Servicios web.

Se despliegan las instancias sa_user_ss y sa_bank_ss en la instancia de AWS

![01](img/lab6_01.png)

Luego, se realiza la verificación del consumo de los servicios web:
#### sa_bank_ss:

![02](img/lab6_02.png)

![03](img/lab6_03.png)

#### sa_user_ss:

![04](img/lab6_04.png)

![05](img/lab6_05.png)

### 2. Creación y configuración del Bus Empresarial de Servicios.

Se crea el modulo BPEL, añade el servidor de openESB y se inicia

![06](img/lab6_06.png)

![07](img/lab6_07.png)

Se añaden las conexiones a los microservicios

![08](img/lab6_08.png)

Se crea el documento WSDL y se le añaden las conexiones previamente realizadas

![09](img/lab6_09.png)

Se realiza el flujo de operaciones que debe ejecutar el modulo BPEL, y posteriormente se configura

![10](img/lab6_10.png)

![11](img/lab6_11.png)

