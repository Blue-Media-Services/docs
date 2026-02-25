# Google Tag Manager

Los gestores de etiquetas son una herramienta gratuita que facilita añadir, gestionar y actualizar códigos de seguimiento (o "etiquetas") en tu sitio web. En este artículo, vamos a hablar de uno de ellos, el más popular y accesible, Google Tag Manager o GTM. Sin embargo, todos funcionan de manera similar, así que no dudes en utilizar el gestor de etiquetas que te resulte más conveniente.

Estos son los temas que se tratan en este artículo:

* [Instalación de GTM](google-tag-manager.md#installing-google-tag-manager)
* [Activadores](google-tag-manager.md#triggers)
* [Variables](google-tag-manager.md#variables)
* [Etiquetas](google-tag-manager.md#tags)
* [Plantillas](google-tag-manager.md#templates)
* [Información Adicional](google-tag-manager.md#additional-information)

## Instalación de Google Tag Manager

Después de crear una cuenta en GTM, debe instalar el código GTM en las páginas de su sitio web. Este código se encuentra en la página de inicio de su contenedor.

<figure><img src="../.gitbook/assets/Captura de tela 2024-11-05 105747.png" alt=""><figcaption><p>Página de inicio de GTM Container</p></figcaption></figure>

Haga clic en el ID del contenedor para abrir las instrucciones de instalación de GTM. Hay dos fragmentos de código que deben instalarse en su sitio web: el primero va en el `<head>`, y el segundo en el `<body>.`

<figure><img src="../.gitbook/assets/image (808).png" alt=""><figcaption><p>Instrucciones de instalación de GTM</p></figcaption></figure>

Después de instalar los códigos GTM, podrás probar tu sitio web para asegurarte de que la instalación se haya realizado correctamente.

## Activadores

Configurar los activadores es fundamental para supervisar acciones o eventos específicos en su sitio web. Los activadores determinan cuándo y dónde deben activarse sus etiquetas, lo que le permite gestionar los datos recopilados para cada interacción del usuario.

Puedes configurar los activadores en la página Activadores o mientras creas o editas una etiqueta.

<figure><img src="../.gitbook/assets/image (809).png" alt=""><figcaption><p>Página de Activadores</p></figcaption></figure>

GTM ofrece varios tipos de activadores para capturar diferentes acciones de los usuarios. Estos son los más utilizados en el seguimiento del comercio electrónico:

1. **Vista de página:** Se activa cuando se carga una página.
2. **Clic:** Se activa cuando se hace clic en un elemento específico de una página, como el botón "Añadir al carrito".
3. **Envío de formulario:** Se activa cuando se envía un formulario de la página.
4. **Evento personalizado:** Se activa en función de eventos JavaScript personalizados, que son útiles para interacciones complejas que no tienen activadores GTM directos.
5. **DOM Ready:** Se activa cuando se carga el HTML de la página (antes que las imágenes y otros medios).

Puedes obtener más información sobre todos los tipos de activadores en este GTM [artículo](https://support.google.com/tagmanager/topic/7679108?sjid=9288738402311135972-SA).

### Configuración de Activadores

Ahora, veamos algunos ejemplos que te ayudarán a comprender cómo configurar los activadores:

_**Ejemplo 1:** Configuración de un activador Añadir al carrito_

Objetivo: Activar una etiqueta cuando un usuario haga clic en el botón "Añadir al carrito".

1. Identifica el selector CSS o el ID del botón:
   * Haga clic con el botón derecho en el botón "Add to Cart" (Añadir al carrito) de su sitio web y seleccione "Inspeccionar". Busque el selector CSS único, el ID o la clase correspondiente al botón (como por ejemplo  `.example` o `#example`).
2.  Crea el activador en GTM:

    <figure><img src="../.gitbook/assets/image (820).png" alt=""><figcaption><p>Configuración del disparador</p></figcaption></figure>

    * Haga clic en <img src="../.gitbook/assets/image (810).png" alt="" data-size="line"> y luego <img src="../.gitbook/assets/image (811).png" alt="" data-size="original"> para comenzar a configurar tu activador.
    * Seleccionar Hacer clic - Todos los elementos si el botón no es un enlace, o Hacer clic - Solo enlaces si se trata de un enlace.
    * En Tipo de activación, selecciona Algunos clics.
    * Establece las condiciones para que coincidan con el selector o el ID del botón. Por ejemplo:
      * Haga clic en Elemento > Selector CSS > `.example`.
    * Guarde el activador y asígnele un nombre descriptivo, como **Añadir al carrito.**
3. Asignar activador a una etiqueta:
   * Añade este activador a la etiqueta **Añadir al carrito** que has creado, para que solo se active cuando se haga clic en este botón.

_**Ejemplo 2:** Configuración de un desencadenante de compra_

**Objetivo:** Activar una etiqueta cuando um usuario completa una compra (normalmente en una página de "Gracias" o "Confirmación de pedido").

1. Utiliza la URL de la página de agradecimiento:
   * Busca la URL única o el patrón de URL de la página de confirmación del pedido. (e.g., `/thank-you` o `/order-confirmation`).
2.  Crear un activador de vista de página:

    <figure><img src="../.gitbook/assets/image (821).png" alt=""><figcaption><p>Configuración del disparador</p></figcaption></figure>

    * Haga clic en <img src="../.gitbook/assets/image (810).png" alt="" data-size="line"> y luego <img src="../.gitbook/assets/image (811).png" alt="" data-size="original"> para comenzar a configurar tu activador.
    * Seleccione Vista de página como tipo de activador.
    * Seleccionar algunas vistas de página.
    * Establece la condición para que coincida con la URL de la página de agradecimiento:
      * Ruta de la página > contiene > `/thank-you`.
    * Guarde el desencadenador como Desencadenador de confirmación de compra.
3. Adjuntar desencadenante a la etiqueta de compra:
   * Asigna este activador a tu etiqueta Producto pedido para realizar un seguimiento de las compras completadas.

_**Ejemplo 3:** Uso de un desencadenador de eventos personalizado para acciones avanzadas_

**Objetivo:** Activar una etiqueta para acciones que no coinciden con los desencadenantes estándar, como eventos JavaScript personalizados.

1. Implementar un evento personalizado:
   *   Si su plataforma de comercio electrónico o desarrollador puede añadir eventos JavaScript personalizados, puede utilizar un JavaScript  `dataLayer.push`  evento. Por ejemplo:

       ```javascript
       dataLayer.push({
         event: 'addToCart',
         productID: '12345',
         productName: 'Sample Product'
       });
       ```
2.  Crear un desencadenador de eventos personalizado:

    <figure><img src="../.gitbook/assets/Captura de tela 2024-11-05 121903.png" alt=""><figcaption><p>Desencadenador de eventos personalizado</p></figcaption></figure>

    * Haga clic en <img src="../.gitbook/assets/image (810).png" alt="" data-size="line"> y luego <img src="../.gitbook/assets/image (811).png" alt="" data-size="original"> para comenzar a configurar tu activador.
    * Seleccione Evento personalizado como tipo de activador.
    * En el campo Nombre del evento, introduzca el nombre del evento utilizado en el `dataLayer.push`, como `addToCart`.
    * Guarde este activador como un activador de evento personalizado Añadir al carrito.

## Variables

En GTM, las variables se utilizan para almacenar información que puede utilizarse en etiquetas, activadores y otras variables. Mejoran la funcionalidad de las etiquetas y los activadores, ya que permiten ajustarlos dinámicamente en función de las acciones del usuario o los datos presentes en la página.

<figure><img src="../.gitbook/assets/image (812).png" alt=""><figcaption><p>Página de variables</p></figcaption></figure>

### Comprender los tipos de Variables

Hay dos tipos de variables disponibles en GTM:

1. **Variables integradas:** GTM proporciona variables integradas para acciones comunes, como la URL de la página, la URL de clic y el ID del formulario. Puede habilitarlas directamente en GTM.
2. **Variables definidas por el usuario:** Son variables personalizadas que se crean para capturar datos específicos, como el ID de un producto o una clase de clic de botón. Los tipos de variables definidas por el usuario incluyen:
   * **Variables de la capa de datos:** Recuperar los valores introducidos en la `dataLayer` (por ejemplo, un ID de producto del código de su sitio web).
   * **Variables URL:** Captura datos de la URL de la página, como parámetros (por ejemplo, parámetros como `utm_campaign`).
   * **Variables JavaScript:** Recupera valores directamente de expresiones JavaScript (por ejemplo, propiedades de objetos de documentos).
   * **Variables constantes:** Almacenan valores fijos (por ejemplo, un ID de seguimiento estático utilizado en varias etiquetas).

### Configuración de Variables

1. **Variables integradas**
   * En la sección **Variables integradas**, haga clic en <img src="../.gitbook/assets/image (900).png" alt="" data-size="line">.
   * Seleccione las variables que desea habilitar marcando sus casillas (por ejemplo, URL de la página, URL de clic, Texto de clic, ID del formulario).
2.  **Variables definidas por el usuario**

    *   _**Ejemplo 1:** Creación de una variable de capa de datos_

        Las variables de la capa de datos extraen los datos que se han enviado a la `dataLayer`. Esto resulta útil cuando se realiza un seguimiento de acciones o valores específicos, como el ID de un producto o una categoría.

        1.  **Enviar datos a la capa de datos** (si aún no se ha hecho):\
            En su sitio web, asegúrese de que los datos necesarios se envían al  `dataLayer`. Aquí hay un ejemplo para una página de producto:

            ```javascript
            dataLayer.push({
                event: 'productViewed',
                productID: '12345'  // Unique identifier for the product
            });
            ```
        2.  **Cree la variable de capa de datos en GTM:**

            <figure><img src="../.gitbook/assets/image (901).png" alt=""><figcaption><p>Configuración variable: Ejemplo de capa de datos</p></figcaption></figure>

            * En la sección Variables definidas por el usuario, haga clic en <img src="../.gitbook/assets/image (816).png" alt="" data-size="line">.
            * Seleccione Configuración variable y elija Variable de capa de datos.
            * En Nombre de variable de capa de datos, introduzca el nombre utilizado en su envío de capa de datos (por ejemplo, `productID`).
            * Opcionalmente, establezca un valor predeterminado si la variable está vacía (por ejemplo, `unknown`).
            * Asigne un nombre y guarde la variable (por ejemplo, DL - ID del producto).
        3. **Prueba:** Utiliza el modo de vista previa de GTM para comprobar que la variable captura correctamente el ID del producto.
    * _**Ejemplo 2:** Creación de una variable URL_

    <figure><img src="../.gitbook/assets/image (382).png" alt=""><figcaption><p>Configuración variable - Ejemplo de URL</p></figcaption></figure>

Las variables URL te permiten capturar datos de la URL de la página, como parámetros de seguimiento (`utm_campaign`) o rutas de páginas específicas.

1. En la sección Variables definidas por el usuario, haga clic en <img src="../.gitbook/assets/image (816).png" alt="" data-size="line">.
2. Seleccione Configuración variable y seleccione URL.
3. En el menú desplegable Tipo de componente, elige la parte de la URL que necesitas:
   * Ruta de la página: Captura la ruta después del dominio (por ejemplo, `/products/shoes`).
   * Consulta: Captura parámetros URL específicos como `utm_campaign`.
4. Si elige Consulta, introduzca la clave de consulta (por ejemplo, `utm_campaign`).
5. Guarda la variable con un nombre descriptivo, como URL - Campaña UTM.

### Uso de Variables

Después de crear variables, puedes utilizarlas para hacer que las etiquetas y los activadores sean más dinámicos.

1. **En Etiquetas:** Al configurar una etiqueta, puede insertar variables seleccionando el símbolo \{{\}} o escribiendo \{{nombre de la variable\}}. Por ejemplo:
   * Utiliza \{{GA Tracking ID\}} en una etiqueta de Google Analytics para el campo ID de seguimiento.
   * Utiliza \{{DL - ID del producto\}} para pasar dinámicamente el ID del producto en una etiqueta de conversión.
2. **En los Activadores:** Las variables se pueden utilizar en los desencadenadores para especificar las condiciones de activación. Por ejemplo:
   * Crear un activador que se dispare en las páginas donde \{{URL - Ruta de la página\}} contenga /checkout.

## Etiquetas

Las etiquetas son fragmentos de código que se utilizan para recopilar datos y supervisar las interacciones de los usuarios para plataformas de marketing y análisis. En lugar de insertar manualmente cada etiqueta en el código de su sitio web, GTM actúa como un centro neurálgico que le permite gestionar todas sus etiquetas en un solo lugar.

<figure><img src="../.gitbook/assets/image (822).png" alt=""><figcaption><p>Página de etiquetas</p></figcaption></figure>

### Creación de Etiquetas

Hay muchas cosas que se pueden lograr utilizando etiquetas. GTM ofrece varios tipos de etiquetas. A continuación se muestra un ejemplo de cómo crear una etiqueta utilizando los códigos de píxeles de BMS.

<figure><img src="../.gitbook/assets/image (825).png" alt=""><figcaption><p>Configuración de etiquetas</p></figcaption></figure>

1. En la página Etiquetas, haga clic en <img src="../.gitbook/assets/image (823).png" alt="" data-size="line"> para añadir una nueva etiqueta y luego en <img src="../.gitbook/assets/image (827).png" alt="" data-size="line"> para comenzar a configurarlo.
2. Selecciona HTML personalizado en la lista.
3. En el campo HTML, pega el código de píxel que necesitas instalar. En el ejemplo, se utilizó un píxel de producto añadido al carrito.
4. Recuerde sustituir el ID de la oferta por la variable identificadora del producto utilizada en su sitio web o utilice una variable GTM previamente configurada vinculada a ella. Puede obtener más información sobre cómo funciona el BMS OfferID en nuestro [Catálogos](../product-documentation/catalog-storage-service-cs2/catalogs.md#install-instructions) artículo.
5.  Seleccione los desencadenantes que controlarán cuándo se activará esta etiqueta.

    <figure><img src="../.gitbook/assets/image (828).png" alt=""><figcaption></figcaption></figure>
6. Nombra y guarda tu etiqueta.
7. Haga clic en <img src="../.gitbook/assets/image (830).png" alt="" data-size="line"> para acceder a una vista previa de tu página con las etiquetas instaladas y depurarlas si es necesario. (Este paso es opcional).
8. Haga clic en <img src="../.gitbook/assets/Captura de tela 2025-04-24 103600.png" alt="" data-size="line"> para enviar los cambios a la versión activa de su sitio web.

## Plantillas

Como alternativa, puede utilizar nuestra plantilla BMS Universal Tag para instalar fácilmente los componentes BMS en su sitio web. Esta única plantilla contiene la mayoría de nuestras etiquetas de productos, y discutiremos más adelante las acciones disponibles.

### Configuración de la etiqueta universal BMS

Al crear una nueva etiqueta, deberá elegir el tipo de etiqueta. Aquí es donde encontrará nuestra plantilla después de buscarla como "Etiqueta universal BMS".

<figure><img src="../.gitbook/assets/image (1092).png" alt=""><figcaption><p>Seleccionar tipo de etiqueta - Búsqueda de etiqueta universal BMS</p></figcaption></figure>

Después de seleccionar esta plantilla, deberá completar algunos datos según la acción que necesite ejecutar. Estas son algunas de las acciones disponibles:

* [Seguimiento de la carga de la página](google-tag-manager.md#track-page-loaded)
* [Añadir usuario a Cookie Pool](google-tag-manager.md#add-user-to-a-cookie-pool)
* [Registrar la actividad del usuario en un Rastreador](google-tag-manager.md#record-user-activity-in-a-tracker)
* [Contar eventos en el Catálogo](google-tag-manager.md#count-event-in-a-catalog)
* [Contenedor de Etiquetas](google-tag-manager.md#tag-container)

#### Seguimiento de la carga de la página

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103042.png" alt=""><figcaption><p>Seguimiento de la carga de la página</p></figcaption></figure>

Cuando se active, esta acción ejecutará el [Etiqueta de Seguimiento de Carga de Página](../product-documentation/ad-server/page-load-tracking-tag.md). Para configurarlo, deberá rellenar los siguientes datos:

* **ID de cuenta BMS:** Su número de cuenta BMS de 12 dígitos.

#### Añadir usuario a Cookie Pool

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103323.png" alt=""><figcaption><p>Añadir usuario a Cookie Pool</p></figcaption></figure>

Cuando se active, esta acción añadirá usuarios a un [Cookie Pool](../product-documentation/data-management-platform-dmp/cookie-pools.md). Para configurarlo, deberá rellenar los siguientes datos:

* **ID de cuenta BMS:** Su número de cuenta BMS de 12 dígitos.
* **ID de Cookie Pool:** Inserte su ID de Cookie Pool; este se encontra disponible al crear o editar un cookie pool en el editor de cookie pools.

#### Registrar la actividad del usuario en un Rastreador

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103424.png" alt=""><figcaption><p>Registrar la actividad del usuario en un Rastreador</p></figcaption></figure>

Cuando se active, esta acción ejecutará tu [Rastreador](../product-documentation/data-management-platform-dmp/trackers/) acciones. Para configurarlo, deberá rellenar los siguientes datos:

* **ID de cuenta BMS:** Su número de cuenta BMS de 12 dígitos.
* **ID del Rastreador:** Introduce tu ID del rastreador; está disponible al crear o editar un rastreador en el editor de rastreadores. También puedes utilizar una variable de tu sitio web que proporcione tu ID del rastreador cuando se active.
* **ID del Evento:** Introduzca la variable que haya identificado como el ID del evento que desea capturar.
* **Datos personalizados:** Si ha configurado campos de datos personalizados en su BMS Tracker, añádalos aquí.

#### Contar eventos en el Catálogo

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103516.png" alt=""><figcaption><p>Contar eventos en el Catálogo</p></figcaption></figure>

Cuando se active, esta acción cargará tu [Catálogos](../product-documentation/catalog-storage-service-cs2/catalogs.md) píxel en tu sitio web. Para configurarlo, deberás rellenar los siguientes datos:

* **ID de cuenta BMS:** Su número de cuenta BMS de 12 dígitos.
* **Evento:** Seleccione el evento que desea capturar en el menú desplegable.
* **ID del Catálogo:** Puede insertar el ID de su catálogo o una variable de su sitio web que proporcione el ID cuando se le solicite.
* **ID del Producto:** Inserte una variable de su sitio web que proporcione el ID del producto cuando se solicite.

#### Contenedor de Etiquetas

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-22 102738.png" alt=""><figcaption><p>Contenedor de Etiquetas</p></figcaption></figure>

Cuando se active, esta acción cargará un [Contenedor de Etiquetas](google-tag-manager.md#tag-container) en su sitio web. Para configurarlo, deberá rellenar los siguientes datos:

* **ID de cuenta BMS:** Su número de cuenta BMS de 12 dígitos.
* **ID del contenedor de Etiquetas:** Introduzca el ID del contenedor de etiquetas BMS.
* **Datos personalizados:** Si ha configurado campos de datos personalizados para este contenedor de etiquetas, añádalos aquí.

## Información Adicional

Cada sitio de comercio electrónico o sitio web tiene sus propias particularidades. Para configurar Google Tag Manager correctamente, es importante tener en cuenta estos detalles. Puede obtener más información sobre algunas de estas plataformas de comercio electrónico en los siguientes enlaces:

* [Cómo usar GTM en Nuvemshop](https://atendimento.nuvemshop.com.br/pt_BR/12313-codigos-externos/como-instalar-google-tag-manager-gtm-na-nuvemshop)
* [Cómo usar GTM en Shopify](https://help.shopify.com/en/manual/promoting-marketing/pixels/custom-pixels/gtm-tutorial)
* [Cómo usar GTM en Wix](https://support.wix.com/en/article/connecting-your-google-tag-manager-account-to-your-wix-site)

Echa un vistazo a estos artículos para obtener más información sobre cómo funciona tu sitio web o plataforma de comercio electrónico, y los nombres que utilizan para eventos, identificadores de productos, etc.
