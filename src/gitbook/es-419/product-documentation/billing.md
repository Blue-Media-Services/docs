# Facturación

Dado que BMS es una plataforma de autoservicio, nuestra facturación funciona de manera diferente, ofreciendo más transparencia en la presentación de sus facturas. La mayoría de las plataformas no proporcionan información detallada sobre cada servicio utilizado, lo que puede dar la impresión de que algunos servicios no se están cobrando. Sin embargo, es importante entender que cada acceso, llamada a la API y archivo almacenado en una plataforma genera un coste.

BMS cree que mostrar a los usuarios la cantidad exacta que pagan por cada servicio es esencial para la transparencia. Al hacer esto, los usuarios pueden identificar dónde se gasta la mayor parte de su dinero y tomar decisiones estratégicas basadas en esa información.

_**Ejemplo:** Al consultar el menú de un restaurante, este normalmente no indica el coste de cada ingrediente individual de un plato; solo muestra el precio total. Sin embargo, en BMS, cada ingrediente, la cantidad solicitada y el coste de cada uno se muestran de forma transparente, permitiéndole decidir qué ingredientes consumirá._

Todos nuestros productos incluirán información detallada sobre el coste de cada servicio utilizado. BMS no cobrará por funciones o productos que no esté utilizando.

Para acceder a sus facturas, haga clic en el menú desplegable de su cuenta y, a continuación, haga clic en <img src="../.gitbook/assets/image (605).png" alt="Billing" data-size="line">.

<figure><img src="../.gitbook/assets/image (518).png" alt=""><figcaption><p>Acceso a facturación</p></figcaption></figure>

Una vez que acceda a la página de facturas, se le mostrarán las facturas del mes actual.

<figure><img src="../.gitbook/assets/image (746).png" alt=""><figcaption><p>Facturas</p></figcaption></figure>

BMS cuenta con varias unidades para contabilizar con precisión cada servicio. Cada unidad funciona de manera diferente para presentar el recuento correcto de uso. A continuación, encontrará una tabla con información detallada sobre el funcionamiento de cada unidad.

| Unidades cargadas               | Descripción                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Solicitudes**                 | Cada acción realizada en BMS cuenta como una solicitud. Esto significa que cada vez que accede a sus creatividades, hace clic en "crear una creatividad" o enumera sus campañas, todas estas acciones contarán como solicitudes.                                                                                                                                                                                                          |
| **Tiempo Transcurrido (horas)** | Todos los datos almacenados en BMS, desde las campañas creadas hasta los archivos multimedia guardados en su biblioteca, generan un coste. BMS factura basándose en el tiempo transcurrido de todos los datos hasta que estos son eliminados. El tiempo transcurrido en BMS se mide en **segundos** y luego se convierte a **horas**, garantizando que usted solo pague por el tiempo exacto que utiliza los servidores de BMS.           |
| **Bytes**                       | Los archivos almacenados en BMS, que se guardan o procesan una vez que un anuncio ha sido descargado en el navegador del usuario final, generan un coste debido a que se accede a ellos desde los servidores de BMS. Los archivos almacenados se cobran en función de su **tamaño en bytes** y la **duración** del tiempo que permanecen guardados. Por otro lado, los archivos descargados se cobran únicamente en función de su tamaño. |
| **Puntos**                      | Estos se basan en métricas. Cada **punto** marcado en sus métricas se registra y se suma con otras métricas; así es como se facturan las métricas.                                                                                                                                                                                                                                                                                        |
| **Eventos**                     | En la pestaña de monitoreo, se encuentran los **conductos de eventos** (event pipes) y los almacenes (event stores). Cada evento registrado desde los almacenes y conductos creados será contabilizado y, posteriormente, se facturará en función del número total de eventos procesados.                                                                                                                                                 |

## Resumen

* ID de cuenta - Facturas de la ID de cuenta actual.
* Periodo - El periodo en el que se seleccionan las facturas actuales.
* Última actualización - Muestra cuándo se actualizaron por última vez los cargos por servicio.
* Estado - El estado actual de la factura seleccionada. Una vez cerrada la factura del mes seleccionado, se mostrará con el estado actual.

## Cargos por Servicio

En esta sección se enumerarán todos los productos. Después de hacer clic en <img src="../.gitbook/assets/image (606).png" alt="Dropdown menu" data-size="line"> , la lista se ampliará para mostrar todos los cargos relacionados con ese producto. Puede comprobar cada producto por separado o hacer clic en <img src="../.gitbook/assets/image (607).png" alt="Expand All" data-size="line"> para ver todos los productos a la vez.

Al ampliar un producto, verá una vista detallada de cada servicio utilizado dentro de ese producto. Esta opción proporcionada por BMS permite a los usuarios controlar sus gastos e identificar áreas para evitar usos innecesarios. Gracias a la transparencia de BMS, los usuarios pueden consultar todos los servicios utilizados, el precio total y la cantidad de uso procesado.

## Cargos por Cuenta

Si eres propietario de una organización, verás los cargos de cada cuenta, con la posibilidad de revisar todos los elementos que figuran en cada cuenta. Esto te proporciona total transparencia e información sobre cada cuenta dentro de la organización.

<figure><img src="../.gitbook/assets/image (651).png" alt=""><figcaption><p>Cargos por Cuenta detallados</p></figcaption></figure>

## Niveles Gratuitos

En BMS, la mayoría de los servicios incluyen una cierta cantidad de uso gratuito. Una vez superado el nivel gratuito establecido, se aplicarán cargos. Por ejemplo, la mayoría de las solicitudes permiten hasta 1000 solicitudes gratuitas; más allá de eso, se incurrirá en cargos adicionales por cada 1000 solicitudes posteriores.

Al crear una campaña, algunas funciones incluyen niveles gratuitos relacionados con el almacenamiento, lo que le permite ejecutar campañas básicas sin costes para determinados elementos de almacenamiento. Los detalles del nivel gratuito son los siguientes:

* **DSP**
  * **Campañas:** 5 Campañas al mes (3,600 campañas-hora) - Gratis
* **Ad Server**
  * **Anuncios almacenados:** Hasta 30 anuncios al mes (21,600 anuncios-hora) - Gratis
  * **Grupos de creatividades almacenados:** Hasta 30 grupos de creatividades al mes (21,600 grupos-de-creatividades-hora) - Gratis
  * **Creatividades almacenadas:** Hasta 30 creatividades al mes (21,600 creatividades-hora) - Gratis

## Modelos de Uso

El BMS tiene dos tipos de uso: **Facturación Discreta** y **Facturación Continua.**

### Modelo de Peaje (Facturación Discreta)

La facturación discreta se refiere a un modelo de uso en el que los cargos se aplican por acciones o eventos específicos a medida que se producen, en lugar de hacerlo de forma recurrente o con una tarifa plana. Este modelo se centra en la transparencia y la precisión en la facturación, garantizando que los usuarios paguen exactamente por los recursos y servicios que consumen. Por ejemplo, al acceder a un producto y realizar acciones como crear, ver o solicitar informes, cada acción se contará como una llamada o solicitud de API. Dado que BMS es una plataforma transparente, todas las solicitudes se mostrarán en la factura del producto correspondiente.&#x20;

La plataforma de BMS consta de múltiples API. Cada vez que accede a un producto y realiza alguna acción, se cuenta como una llamada a la API, lo que indica que se ha utilizado la API. BMS se refiere a una llamada a la API como una solicitud, y se reflejará en su factura bajo el producto correspondiente al que ha accedido e interactuado.

Este tipo de uso se basa en un sistema de **peaje**. Cada vez que accedes a una página, pasas por un peaje y se te cobra por acceder a la página del producto. Si realizas cualquier acción en la misma página, también se contará como pasar por un peaje, por lo que se contará como una solicitud.

_**Ejemplo:** Si accede a la biblioteca multimedia y sube un archivo multimedia, se contará como una solicitud. Del mismo modo, descargar ese archivo multimedia también se contará como una solicitud. Después de subir una imagen, si envía el enlace de la imagen a otra persona y esta accede a la imagen, también se le cobrará, ya que la imagen está alojada en los servidores de BMS y vinculada a su cuenta._

A continuación encontrará algunas solicitudes que se ajustan a nuestro modelo de uso discreto.

<figure><img src="../.gitbook/assets/image (610).png" alt=""><figcaption><p>Ejemplo de solicitudes</p></figcaption></figure>

_**Ejemplo:** Las líneas "Get Ad - First 1,000 - free" (Obtener anuncio - Primeras 1,000 - gratis) y "Get Ad - After 1,000 - $0.01 per 1,000" (Obtener anuncio - Después de 1,000 - $0.01 por cada 1,000) se refieren al mismo servicio. Esto significa que usted dispone de 1,000 solicitudes gratuitas y, una vez superadas, se le facturará 0.01 USD por cada 1,000 solicitudes adicionales._

### Modelo de Estacionamiento (Facturación Continua)

Como resultado de la facturación discreta, cuando usted accede, crea y gestiona funciones en BMS, cualquier archivo multimedia subido, así como las campañas, anuncios y creatividades creadas y almacenadas, consumirán espacio en los servidores de BMS. BMS incurre en costes por el uso de este espacio y, aunque todos los datos se almacenen en la nube, existe un coste asociado que el usuario debe abonar.

Mientras que todas las plataformas cobran por el espacio utilizado, BMS destaca por mostrar de forma transparente exactamente dónde está consumiendo espacio el usuario. Esta transparencia permite a los usuarios tomar decisiones informadas sobre si reducir el uso de un producto o decidir almacenar sus archivos multimedia en sus propios servidores para evitar dichos cargos.

Este modelo se basa en el uso en tiempo real de BMS, contabilizando el tiempo que una función está activamente en uso. Por ejemplo, una campaña activa durante todo un mes se facturará por 720 horas de uso. Si ejecuta dos campañas durante medio mes y luego las desactiva, también se le cobrarán 720 horas, ya que el uso combinado de ambas sumará ese total. BMS mide el tiempo de uso en segundos, pero para fines de facturación, se convierte a horas. Por lo tanto, solo se le cobrará por el tiempo real en que una función esté en uso.

Las creaciones consumen espacio porque se alojan en el servidor de BMS; por lo tanto, el cargo se basará en la cantidad de espacio utilizado.

Este uso puede relacionarse con el uso de un **estacionamiento**: Una vez que llegas con tu coche al estacionamiento, se te empieza a cobrar por el tiempo transcurrido. Puedes identificar el coche como una creatividad que se ha creado y el estacionamiento como BMS. Cada segundo que tu coche permanece en el estacionamiento, BMS lo cuenta, y una vez que retiras tu coche, deja de cobrarte.

_**Ejemplo:** Una vez que sube un archivo multimedia de 1 MB, BMS comenzará a rastrear cuánto tiempo permanece almacenado y cobrará por este archivo mientras se mantenga en el servidor. Si conserva 1 MB de contenido durante un mes, la factura se basará en el periodo total en segundos y la cantidad de datos almacenados. Si elimina el archivo, BMS dejará de cobrar por él, ya que dejará de consumir espacio._
