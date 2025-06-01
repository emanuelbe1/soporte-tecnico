### Modelo TCP/IP de cinco capas
<p>En ciencias de la computación, el concepto de capas de red conforma una estructura que ayuda a entender las interacciones complejas en las redes informáticas.</p>

<p>El modelo TCP/IP de cinco capas es el propuesto por los autores **Behrouz A. Forouzan** y **James Kurose**, y es el que se utiliza en el curso **Google IT Support Professional** (fuente principal de la cuál se toma este apunte). Es útil para comprender la arquitectura de internet y los protocolos involucrados en la comunicación entre dispositivos. Existen otros modelos, variando entre tres (*RFC 871*) a siete capas (*ISO/IEC 7498-1:1994*).</p>

El modelo de cinco capas consta de:
- Capa física
- Capa de enlace de datos
- Capa de red
- Capa de transporte
- Capa de aplicación

<ul>
<li>El modelo OSI es el más conocido. Es el que se utiliza en certificaciones **CompTIA Net+** y **Cisco CCNA**.</li>
<li>El modelo TCP/IP tradicional cuenta con solo cuatro capas, ya que no diferencia entre la capa física y la capa de enlace de datos.</li>
<li>El modelo OSI se diferencia del modelo de 5 capas debido a que divide la capa de aplicación en otras tres capas (Sesión, Presentación y Aplicación)</li>
<li>En lugar de pensarlas literalmente se las puede considerar como capas de complejidad.</li>
</ul>

El modelo de cinco capas consta de:

- Capa física
- Capa de enlace de datos
- Capa de red
- Capa de transporte
- Capa de aplicación

#### Primera capa: capa física (*physical layer*)
<p>&nbsp;La capa física de una red representa los dispositivos físicos que interconectan sistemas informáticos. Esto incluye las especificaciones de cables para red y los conectores que los unen, junto con las especificaciones que describen cómo se envían señales por medio de estas conexiones. En su mayoría, se compone de: cableado, conectores y transmisión de señales.</p>

#### Segunda capa: capa de enlace de datos (*data link layer*)
 Algunos recursos también la llaman "interfaz de red" o "capa de acceso a la red". En esta capa se introducen los primeros protocolos. La **capa de enlace de datos** es responsable de definir una forma común de interpretar las señales (de la capa física), para que los dispositivos de red puedan comunicarse.

 Existen muchos protocolos en esta capa, pero el más común es **Ethernet**, aunque las tecnologías inalámbricas se están volviendo más populares.

 Además de especificar atributos de la capa física, el estándar Ethernet define un protocolo responsable de llevar datos a nodos en la misma red o enlace.


##### Tercera capa: capa de red (*network layer*)
<p>Esta capa aveces es llamada **capa de Internet**. Esto es porque permite que diferentes redes se comuniquen entre sí a través de dispositivos popularmente conocidos como **routers**.</p>

<p>Un conjunto de redes conectadas entre sí a través de routers es una **internetwork**, siendo la más famosa **Internet**. Mientras que la *capa de enlace de datos* es responsable de mover datos en un enlace individual, la *capa de red* se encarga de enviarlos a través de un conjunto de redes.</p>

<p>La capa de red, por lo tanto, entrega los datos entre dos nodos individuales. El protocolo más común usado en esta capa es **IP** o *Internet Protocol*.</p>


##### Clientes y servidores
El software de redes se divide en categorías de **cliente** y **servidor**. La aplicación cliente inicia la solicitud (*request*) de datos, y el software servidor responde a esta a través de la red. Un solo nodo puede estar ejecutando múltiples aplicaciones cliente o servidor.

#### 4. Capa de transporte (*transport layer*)
 La capa de transporte determina qué programa cliente o servidor debe recibir los datos datos entregados por la capa de red. 
 El protocolo más comúnmente usado en esta capa es **TCP** o *Transmission Control Protocol*. 

	 Si bien es frecuente que se diga "TCP/IP" (todo junto) para resolver problemas de red y por sencillez, es importante saber que estos protocolos son distintos y cumplen propósitos diferentes.

<b>UDP</b>
 Hay otros protocolos de transporte además de TCP que utilizan IP, como **UDP** o *User Datagram Protocol*. La principal diferencia es que UDP no provee mecanismos para asegurarse que los datos se entregan correctamente.
 *(Posteriormente se verán las diferencias entre TCP y UDP.)*

- [!] La capa de red (en este caso, IP) se encarga de que los datos viajen de un nodo a otro.
- [!] La capa de transporte (TCP/UDP) se asegura de que los datos lleguen a la aplicación correcta en cada nodo. 
- [!] <b>nodo</b>: cualquier dispositivo conectado a la red que puede enviar, recibir o reenviar información. 


##### 5. Capa de aplicación
 Hay muchos protocolos diferentes en esta capa, las cuales son específicos de cada aplicación. Los protocolos usados para permitir la navegación web o enviar y recibir correos son algunos de los más comunes.

##### ¿Abstracción?
Se puede pensar en las capas como distintos aspectos de un paquete a ser entregado.
1. La capa física es el camión de entrega y las carreteras. 
2. La capa de enlace de datos es la forma en que el camión va de una esquina a otra.
3. La capa de red identifica cuáles carreteras se necesitan tomar para llegar de la dirección A a la dirección B.
4. La capa de transporte se asegura de que el conductor sepa cómo tocar la puerta para avisar que llegó
5. La capa de aplicación es el paquete en sí mismo.
