# DMZ_FIREWALL_VPN_PROXY

He empezado creando las 2 máquinas de los firewalls, el firewall externo con un adaptador nat y otro adaptador a la red interna DMZ. El firewall interno con un adaptador a la red DMZ y otro adaptador interno a la red LAN. Por último he instalado el cliente, un windows 10 pro, con un adaptador a la red interna LAN.

## Configuración de interfaces de los Firewalls con pfSense

###  Configuración de las interfaces Firewall Externo

![0](img/0.png)
![1](img/1.png)
![2](img/2.png)

###  Configuración de las interfaces Firewall Interno

![3](img/3.png)
![4](img/4.png)
![5](img/5.png)

## Configuración del cliente interno

![6](img/6.png)

## Acceder al firewall interno desde el cliente

![7](img/7.png)

### Desbloquear la WAN

![8](img/8.png)

### Comprobar salida a internet desde el cliente

![9](img/9.png)

## Regla de Bloqueo

### Regla de bloqueo de DMZ a LAN

![10](img/10.png)
![11](img/11.png)

### Regla bloqueo youtube

![12](img/12.png)
![13](img/13.png)
![14](img/14.png)


# PARTE DOS

# Instalación del servidor VPN

![15](img/15.png)
![16](img/16.png)
![17](img/17.png)
![18](img/18.png)
![19](img/19.png)
![20](img/20.png)
![21](img/21.png)
![22](img/22.png)
![23](img/23.png)
![24](img/24.png)
![25](img/25.png)
![26](img/26.png)
![27](img/27.png)

## Después de crear el archivo OVPN, lo descargo en el cliente para poder conectarme a la VPN.

![28](img/28.png)
![29](img/29.png)
![30](img/30.png)
![31](img/31.png)

## Para crear el servidor proxy utilizo la misma máquina que aloja el servidor VPN para ahorrar recursos.

![32](img/32.png)
![33](img/33.png)
![34](img/34.png)

## Configuramos el proxy en el cliente.

![35](img/35.png)
![36](img/36.png)

## El error se debe a que en el archivo de configuración no había una ACL que permitiera la entrada del tráfico de la DMZ.

![37](img/37.png)
![38](img/38.png)

## Creamos un archivo para restringir los dominios que queramos. El "." delante del nombre del dominio permite bloquear también los subdominios.

![39](img/39.png)
![40](img/40.png)
![41](img/41.png)
