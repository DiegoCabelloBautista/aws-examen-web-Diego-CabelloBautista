# aws-examen-web-Diego-CabelloBautista
## Paso 1: Crear una VPC en AWS

```bash
Primero cuando entramos accederemos a VPC.
```
![](./img/cap1.jpg)
```bash
En el menu que tendremos en la parte media a la izquierda de la pantalla iremos a Sus VPC.
```
![](./img/cap2.jpg)

```bash
Crearemos una.
```
![](./img/cap3.jpg)

```bash
Pondremos nombre y con la CIRD IPv4.
```
![](./img/cap4.jpg)
```bash
En el menu que nos aparcia a la izquierda iremos a subredes.
```
![](./img/cap5.jpg)
```bash
Crearemos una subred.
```
![](./img/cap6.jpg)

```bash
Asociamos la subred que queramos crear a la VPC que hayamos creado anteriormente.
```
![](./img/cap7.jpg)
```bash
Ponemos nombre a la subred, y le añadimos la ip a el bloque de CIDR de la subred.
```
![](./img/cap8.jpg)

```bash
Realizaremos lo mismo pero con la subred numero 2.
```
![](./img/cap9.png)

```bash
Una vez creadas les habilitaremos la opcion de asignar automaticamente la direccion IPv4.
```
![](./img/cap10.png)
```bash
Marcaremos esta opcion.
```
![](./img/cap11.jpg)
```bash
A continuacion crearemos una puerta de enlace de internet(gateway).
```
![](./img/cap12.jpg)
```bash
Le asignamos el nombre a la puerta de enlace de internet.
```
![](./img/cap13.jpg)

```bash
Cuando creemos la gateway, nos saldra un mensaje en verde y deberemos de darle para asociarle la vpc.
```
![](./img/cap14.jpg)
```bash
Le asignamos la vpc que hayamos creado a el principio.
```
![](./img/cap13-2.jpg)
```bash
Por ultimo en la seccion de VPC tendremos que crear una tabla de enrutamiento.
```
![](./img/cap15.jpg)
```bash
Una vez creada, nos iremos a ruta, editar ruta.
```
![](./img/cap16.jpg)
```bash
Añadimos la direccion 0.0.0.0, Puerta de enlace de internet, y la seleccionamos la gateway que hayamos creado.
```
![](./img/cap17.jpg)
```bash
Tambien tendremos que asociarle las subredes que hemos creado anteriormente.
```
![](./img/cap18.jpg)
```bash
Ya habremos acabado la parte de VPC, tendremos que acceder a EC2.
```
![](./img/cap19.jpg)

```bash
Iremos a Instancias.
```
![](./img/cap20.jpg)

```bash
Lanzaremos una instancia.
```
![](./img/cap21.jpg)

```bash
Primero crearemos la de windows,le asignamos el nombre, y con la ISO 2022 Base.
```
![](./img/cap22.jpg)

```bash
Le asignamos un par de claves.
```
![](./img/cap23.jpg)

```bash
Le tendremos que añadir el tipo de instancia t3.medium
```
![](./img/cap24.jpg)

```bash
En la configuracion de red, la editaremos, le asignamos la vpc, la subred que hayamos creado para ubuntu y el grupo de seguridad.
```
![](./img/cap25.png)

```bash
Le añadimos las reglas de seguridad de entrada.
```
![](./img/cap26.png)

```bash
Y tambien las de salida.
```
![](./img/cap27.jpg)

```bash
Crearemos una más que sera la de Ubuntu, le asignamos el nombre, la ISO.
```
![](./img/cap28.jpg)
```bash
Le asignamos el par de claves y el tipo de instancia.
```
![](./img/cap29.jpg)
```bash
En la configuracion de red, la editaremos, le asignamos la vpc que hayamos creado, la subred de linux, y creamos el grupo de seguirdad.
```
![](./img/cap30.png)

```bash
Le configuramos las reglas de entrada.
```
![](./img/cap31.jpg)

```bash
Y tambien las de salida.
```
![](./img/cap32.jpg)
```bash
Ya tendremos que conectarnos a la maquina virtual, seleccionaremos la maquina virtual, le daremos a conectar y en el apartado de cliente de ssh
```
![](./img/cap33.jpg)

```bash
Una vez dentro tendremos que ejecutar los siguientes comandos
```
![](./img/cap34.jpg)
![](./img/cap35.jpg)
![](./img/cap36.jpg)
![](./img/cap37.jpg)

## Pull request

```bash
Para que mi compañero pueda realizarme un pull request tendre que crear un .txt por ejemplo.
```
![](./img/cap43.png)

```bash
Le añadimos un commit para guardarlo.
```
![](./img/cap44.png)


```bash
Realizaremos un git push origin andres, para subirlo a GitHub y que mi compañero pueda hacerme el Pull Request.
```
![](./img/cap45.png)


```bash
Una vez que hayamos echo lo anterior, tendremos que agregarlo colaboradores, y el a nosotros, cuando nos agregue acceptaremos la solicitud, iremos a su GitHub, y en el apartado de arriba seleccionaremos Pull Request y Create Pull Request.
```
![](./img/cap46.png)


```bash
Le ponemos un titulo y una descripcion.
```
![](./img/cap47.png)


```bash
Ya habriamos realizado el Pull request como podemos comprobar.
```
![](./img/cap48.png)

