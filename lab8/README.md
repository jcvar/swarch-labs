#### Universidad Nacional de Colombia
### Arquitectura de Software
## Laboratorio 8 - Grupo 2E

- Julian David Acosta
- Luis Ferney Sandoval
- Juan Camilo Vargas
- Francisco Javier Bernal
- Santiago Duque Bernal
- Santiago Hernández Montano
- Santiago Alejandro Morales

### 1. Soporte visual del la configración y uso del entorno de pruebas

- En Test Plan, agregar un nuevo Thread Group:
  ![01](img/ss1.png)
- En Test Plan, añadir un nuevo HTTP(s) Test Script Recorder:
  ![02](img/ss2.png)
- Configurar el HTTP(s) Test Script Recorder añadido: 
  ![03](img/ss3.png)
- Iniciar el proceso de grabación en JMeter (Start):\
  En Summary Report observar los resultados de la prueba realizada. Tener en cuenta el tiempo de respuesta.
  ![04](img/ss3.png)

#### Soporte visual de las actividades realizadas durante el desarrollo del Escenario 1

* Usuarios = 1
  ![05](img/sc1/1e1.png)
* Usuarios = 5
  ![06](img/sc1/5e1.png)
* Usuarios = 50
  ![07](img/sc1/50e1.png)
* Usuarios = 75
  ![08](img/sc1/75e1.png)
* Usuarios = 100
  ![09](img/sc1/100e1.png)
* Usuarios = 500
  ![10](img/sc1/500e1.png)
* Usuarios = 750
  ![11](img/sc1/750e1.png)
* Usuarios = 1000
  ![12](img/sc1/1000e1.png)
* Usuarios = 2000
  ![13](img/sc1/2000e1.png)

#### Soporte visual de las actividades realizadas durante el desarrollo del Escenario 2

* Usuarios = 1
  ![14](img/sc2/1e2.png)
* Usuarios = 5
  ![15](img/sc2/5e2.png)
* Usuarios = 50
  ![16](img/sc2/50e2.png)
* Usuarios = 75
  ![17](img/sc2/75e2.png)
* Usuarios = 100
  ![18](img/sc2/100e2.png)
* Usuarios = 500
  ![19](img/sc2/500e2.png)
* Usuarios = 750
  ![20](img/sc2/750e2.png)
* Usuarios = 1000
  ![21](img/sc2/1000e2.png)
* Usuarios = 2000
  ![22](img/sc2/2000e2.png)

#### Tabla y gráfica de rendimiento usando los datos obtenidos en los pasos anteriores, donde se evidencie la curva de rendimiento  para cada uno de los dos escenarios probados

Realizando cada prueba un total de 3 veces, y promediando los resultados de 'Tiempo de Respuesta' obtenidos logramos completar la siguiente tabla:
  ![23](img/tabla.png)

En la siguiente gráfica podemos comparar los resultados obtenidos con cada escenario de prueba:
  ![24](img/grafica.png)

#### Conclusiones

Al observar los resultados obtenidos, a pesar de tener ciertos datos en el **escenario 1** que salen de la tendencia trazada por los puntos obtenidos en las demas pruebas, podemos ver el desempeño significativamente mejor que permite el escalamiento del **escenario 2**.
Entre mayor el número de usuarios concurrentes simulados dentro del sistema, el desempeño del **escenario 2** resulta relativamente mejor al observado sin escalamiento en el **escenario 1**.
De igual forma, vemos que el sistema puede dar una buena respuesta al número de usuarios planteados, ya que dentro del rango de usuarios simulados, no se alcanzan a percibir pérdidas en la respuesta del sistema.
La gráfica obtenida nos muestra que con este rango no se alzanza la rodilla de la curva de rendimiento, es necesario realizar la prueba de carga dentro de un rango de usuarios mayor para determinar su ubicación exacta.

