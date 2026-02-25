---
description: Descubra cómo funciona nuestra pestaña en tiempo real.
---

# Pestaña de Tiempo Real

Los recursos de Anuncios y Campañas cuentan con una pestaña dedicada al monitoreo en tiempo real que permite al cliente ver lo que se está entregando en tiempo real.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-12-30 090101.png" alt=""><figcaption><p>Pestaña en tiempo real que muestra los anuncios que se están mostrando y las interacciones de los usuarios a medida que ocurren.</p></figcaption></figure>

Los eventos disponibles son:

* <img src="../../.gitbook/assets/impression event.png" alt="Impression" data-size="line">\
  Este evento se registra cada vez que una campaña gana el derecho a mostrar un anuncio al usuario final. Este es el momento en el que se cobra el coste de adquisición de medios.
* <img src="../../.gitbook/assets/delivered event.png" alt="Delivered" data-size="line">\
  Este evento se registra cuando el navegador del usuario final solicita el contenido publicitario a nuestro servidor de anuncios. Este es el momento en el que se cobra el coste del servidor de anuncios.
* <img src="../../.gitbook/assets/displayed event.png" alt="Displayed" data-size="line">\
  Este evento se registra cuando el navegador del usuario final carga y muestra el anuncio en una página.
* <img src="../../.gitbook/assets/viewed event.png" alt="Viewed" data-size="line">\
  Este evento se registra cuando al menos el 50 % del cuerpo del anuncio se muestra en la pantalla durante al menos 1 segundo.
* <img src="../../.gitbook/assets/clicked event.png" alt="Clicked" data-size="line">\
  Este evento se registra cuando el usuario final hace clic en el anuncio. Para que se pueda realizar el seguimiento de este evento, debe utilizar el rastreador de clics de BMS, que está habilitado de forma predeterminada, pero que se puede deshabilitar editando el código HTML del creativo.

{% hint style="info" %}
Tenga en cuenta que el evento "impresión" solo se puede rastrear para campañas y anuncios.&#x20;

Al comprobar eventos en tiempo real para creatividades o grupos de creatividades, no se puede registrar ningún evento "impresión". Las reglas publicitarias solo se determinan en el momento de la entrega del anuncio. Este es el momento en el que se selecciona el grupo de creatividades definitivo y, a partir de él, se elige la creatividad definitiva.&#x20;
{% endhint %}

Puedes elegir qué eventos ver cambiando el selector:

<figure><img src="../../.gitbook/assets/image (145).png" alt=""><figcaption><p>Filtro de Eventos</p></figcaption></figure>

Para cualquier evento que aparezca en la lista, puede hacer clic en el botón de detalles ![](<../../.gitbook/assets/image (538).png>) para ver más:

<figure><img src="../../.gitbook/assets/Captura de tela 2024-12-30 090243.png" alt=""><figcaption><p>Pantalla de detalles del Evento</p></figcaption></figure>

Aquí puede observar todos los detalles de un evento concreto, como la geolocalización del usuario, la IP, el navegador y el tipo de dispositivo. Los parámetros de la puja, el intercambio publicitario y el dominio, así como los relacionados con la campaña concreta, el objetivo, el anuncio, la regla publicitaria, el grupo creativo y el creativo, junto con una vista previa del propio creativo.
