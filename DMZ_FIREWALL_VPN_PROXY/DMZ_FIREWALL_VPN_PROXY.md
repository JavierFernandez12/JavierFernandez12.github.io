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