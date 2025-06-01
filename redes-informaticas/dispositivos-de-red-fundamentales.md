## Cables

Conectan distintos dispositivos entre sí, permitiendo que los datos se transmitan a través de ellos.

- Componente más básico de una red cableada

- Se pueden dividir en dos categorías: cobre y fibra, siendo los primeros los más comunes.

#### Cable de cobre
 Se forman por varios ares de cables de cobre dentro de un aislante de plástico. Las forma más comunes de cables de par trenzado usados en redes de computadoras son Cat5, Cat5e y cables Cat6. 

Categorias: Tienen diferentes caracteristicas físicas, como la cantidad de trenzados que dan como resultado diferentes longitudes utilizables y velocidades de transferencia.
- Cat5 es la más antigua, siendo reemplazada por Cat5e y Cat6.
- A simple vista todas se ven iguales.
- La forma en la que se organizan los pares trenzados pueden alterar drásticamente la rapidez de transferencia de datos y la resistencia de estas señales a interferencias externas.	

		El dispositivo emisor comunica los datos binarios a través de estos cables al cambiar el voltaje entre dos rangos. El sistema receptor puede interpretar estos cambios de voltaje y traducirlos en diferentes formas de datos. 

- Cat5e han reemplazado Cat5 debido a que sus componentes internos reducen el *crosstalk*.
	
		Crosstalk: Cuando un pulso eléctrico en un cable es detectado accidentalmente en otro cable



#### Cable de fibra óptica

Contienen fibras opticas individuales. Estas son pequeños tubos hechos de vidrio con, aproximadamente, el ancho de un cabello humano. Estos transportan haces de luz. A diferencia del cobre, no usan voltajes eléctricos: usan pulsos de luz para representar los datos binarios.

 Se suelen usar en entornos donde hay mucha interferencia electromagnética de fuentes externas, ya que puede impactar en los datos que se envien por cables de cobre.
 
 - Generalmente pueden transportar datos más rápido que los cables de cobre, pero son mucho más caros y frágiles.
 - Puede transportar datos a distancias mucho más largas que el cobre sin sufrir perdida de datos. 
 - Es poco probable encontrarse con cables de fibra óptica en casas u oficinas. Son más comunes en centros de datos.
 
## Hubs y Switches
 Los cables permiten crear conexiones de red de punto a punto. Estas son redes donde solo existe un dispositivo en cada extremo del enlace. 
 Hay dispositivos de red que permiten que muchos dispositivos se conecten entre sí. Entre estos entran los hubs y los switches. Son los dispositivos principales que se usan para conectar computadoras en una red de area local (*LAN*).
 
#### Hub o concentrador
  Es un dispositivo de red perteneciente a la *capa física* que posibilita las conexiones de varios dispositivos a la vez. Establece una conexión entre un número indefinido de computadoras, y permite el intercambio de datos. El switch recibe una señal y la repite emitiéndola por sus diferentes puertos. 

- Todos los dispositivos conectados a un hub terminan comunicándose con todos los demás dispositivos al mismo tiempo.
- Depende de cada sistema conectado al hub determinar si los datos entrantes estaban destinados a ellos o ignorarlos si no lo están.
- Esto genera mucho ruido en la red y crea lo que se denomina un dominio de colisión
		
		Dominio de colisión: Un segmento de red donde solo un dispositivo puede comunicarse a la vez
		
 Si muchos sistemas tratan de enviar datos al mismo tiempo, los pulsos eléctricos enviados a través del cable puede interferir uno con el otro. Esto causa que los sistemas entren en un periodo de inactividad antes de volver a intentar enviar sus datos. Debido a la ralentización de las comunicaciones resultante de esto, los hubs son cada vez más raros y en la actualidad son un artefacto histórico.
 
#### Switch o conmutador de red

 Originalmente conocidos como *Switching hubs*. En la actualidad, la tarea del **hub** o *concentrador* las realizan, con frecuencia, los switches. Son dispositivos digitales lógicos para la interconexión de dispositivos. Son una forma mucho más común y sofisticada de conectar varias computadoras, en comparación al *hub*. 
 La diferencia es que el hub es de la capa física (capa 1), mientras que el conmutador o switch es un dispositivo de la capa de enlace de datos (capa 2). Esto significa que el switch puede inspeccionar el contenido de los datos de protocolo Ethernet que estan siendo enviados por la red, determinar a cúal sistema estan dirigidos los datos, y finalmente enviar los datos a ese sistema. 
 
 - Esto reduce o hasta elimina por completo la magnitud del dominio de colisión en la red.
 
 - Esto conlleva a menos retransmisiones y a un throughput mayor. 
 
 
## Routers 
 Los hubs y switches son principales para una red de area local. Sin embargo, con frecuencia se va a querer enviar (o recibir) datos a dispositivos de otras redes. En este aspecto entra el **router**.

 Un **router** es un dispositivo que sabe cómo reenviar datos entre redes independientes. Pertenece a la capa 3: la capa de red. Puede inspeccionar los datos IP para determinar a dónde debe enviar las cosas. 
 
**Tablas de enrutamiento**: Los enrutadores almacenan tablas internas que contienen información sobre cómo enrutar trafico entre diferentes redes en el mundo.


#### Routers de hogar, Residencial Gateway y Core Routers
 El router más común es el que se encuentra en una red doméstica u oficina pequeña. En la actualidad, el router se encuentra integrado en un dispositivo llamado **puerta de enlace**. En este contexto se habla de una puerta de enlace residencial o *residential gateway*. El router se encuentra junto a otros dispositivos integrados como: modem, switch, AP inalámbrico para Wifi, entre otros dispositivos.
 En general, estos no tienen tablas de enrutamiento muy detalladas. La intención principal de estos routers es tomar trafico que se origina de la casa u oficina y reenviarlo al ISP (*Internet Service Provider*).
 
 Una vez que el trafico se envio al ISP, entra en papel un tipo de router más compejo: los core routers. Estos conforman el "backbone" de Internet. Los routers comparten datos con cada uno via un protocolo llamado BGP o *border gateway protocol*. 
 
 
 ## Servidores y clientes
 
