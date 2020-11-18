#### Universidad Nacional de Colombia
### Arquitectura de Software
## Laboratorio 6

- Julian David Acosta
- Luis Ferney Sandoval
- Juan Camilo Vargas

### 1. Despliegue de Servicios web.

Se despliegan las instancias sa_user_ss y sa_bank_ss en la instancia de AWS

![01](img/Lab6_01.png)

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

Se realiza el flujo de operaciones que debe ejecutar el modulo BPEL, se configura y posteriormente se hace el build

![10](img/lab6_10.png)

![11](img/lab6_11.png)

![12](img/lab6_12.png)

### 3. Despliegue del bus de servicios

Ahora se crea la composite application, y se añade el modulo BPEL a la composite application

![13](img/lab6_13.png)

![14](img/lab6_14.png)

Finalmente hacemos el build, y desplegamos

![15](img/lab6_15.png)

![16](img/lab6_17.png)

Y probamos que el servidor está funcionando correctamente

![17](img/lab6_19.png)

### 4. Comprobación de la interoperabilidad

Se verifica que hayan datos en las bases de datos de cada uno de los microservicios

![18](img/lab6_20.png)

![19](img/lab6_21.png)

Posteriormente, se crea el proyecto SOAP para comprobar el funcionamiento del bus de servicios

![19](img/lab6_22.png)

Finalmente, realizamos la transacción entre dos usuarios por una cantidad de 600, y comprobamos que la operación se haya realizado en las bases de datos

![20](img/lab6_23.png)

![21](img/lab6_24.png)



