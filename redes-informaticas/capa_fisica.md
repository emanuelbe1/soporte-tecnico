## Capa física
<p>&nbsp;La <b>capa física</b> consiste en dispositivos y es responsable de la transmisión de bits entre los dispositivos.</p>
<p>&nbsp;Los <b>bits</b> son la representación binaria más pequeña de los datos que una computadora puede comprender. Estos conforman los paquetes que se transmiten a través de la red por medios de la capa física.</p>

#### Modulación
<p>&nbsp;Los bits se envían a través de los cables por medio de un proceso llamado <b>modulación</b>. Este es el proceso mediante el cual se codifican los datos binarios (bits) en señales eléctricas, ópticas o electromagnéticas para que puedan transmitirse eficazmente a través de un medio físico.</p>
 
<p>&nbsp;En redes con cables de cobre, la modulación implica variar el voltaje o la corriente en el conductor. Este tipo de modulación digital se conoce como <b>codificación de linea</b> (<i>line coding</i>).</p>

## Cable de par trenzado y comunicación dúplex
#### Cable de par trenzado

<p>El tipo de cableado más común en redes es el <b>par trenzado</b>. Se llama así porque presenta pares de alambres de cobre que están trenzados entre sí. Estos pares actúan como un único conducto de información y su trenzado ayuda a proteger contra las interferencias electromagnéticas y de otros pares cercanos.</p>

<p>La cantidad de pares usados depende en la tecnología de transmisión. Un cable Cat6 estándar, por ejemplo, consta de cuatro pares trenzados dentro de una sola cobertura aislante.</p>
	
>Es importante notar que, en todas las formas modernas de redes, estos cables permiten la comunicación dúplex.


#### Comunicación duplex
 <p>&nbsp;La <b>comunicación duplex</b> es un sistema que es capaz de mantener una comunicación bidireccional. Es decir, permite enviar y recibir información simultáneamente a través del medio físico (en este caso, el cable de par trenzado).</p>

<p>&nbsp;Por otro lado, existe la <b>comunicación <i>simplex</i></b> que es unidireccional.</p>
<p>&nbsp;Para garantizar una comunicación dúplex, los cables de red suelen reservan uno o dos pares para que transmitir en una dirección y usar los otros uno o dos pares para la dirección opuesta.</p>

<p>Cuando los dispositivos en un enlace de red pueden comunicarse a ambas direcciones al mismo tiempo, se dice que están en <i>full-duplex</i>.</p>

<p>&nbsp;Si un enlace de red se degrada, puede pasar a funcionar en <i>half-duplex</i> lo que significa que solo es posible enviar o recibir información en un momento dado (no ambos a la vez).</p>

## Puertos de red y panel de conexiones
<p>&nbsp;Los cables de red de par trenzado terminan en un conector que toma los cables internos y los expone. El conector más común es conocido como <b>RJ45</b> (<i>Register Jack 45</i>)</p>

#### Puertos de red
<p>&nbsp;Un cable Ethernet con un conector RJ45 puede conectarse a un puerto RJ45.</p>

<p> Un <i>switch</i> tendrá varios puertos de red, ya que su propósito es que se conecten varios dispositivos. Sin embargo, los servidores y las computadoras de escritorio suelen tener uno o dos puertos.</p>

<p>La mayoría de los puertos de red tienen dos pequeñas luces LED. Una indica el <b>enlace</b> (<i>link LED</i>), la otra indica la <b>actividad</b> (<i>activity LED</i>).</p>

> La luz de <i>actividad</i> parpadea cuando los datos se estan transmitiendo activamente a través del cable. En la practica, indica si hay o no algún tipo de trafico.
 
 En switches, aveces se usa un mismo LED para el estado de actividad y enlace.
 
 > Si bien será necesario leer sobre el hardware particular con el que se trabajara, casi siempre estas luces comunican datos útiles para la resolución de problemas.

#### Panel de conexión
<p>En algunos casos, los puertos de red se conectan a un <b>panel de conexión</b> o <i>patch panel</i>. Este es un dispositivo que contiene muchos puertos de red y actuá como un punto de organización central para los cables que van a los switches o routers.</p>
