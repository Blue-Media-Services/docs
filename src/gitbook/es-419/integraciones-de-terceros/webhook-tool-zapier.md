# Herramienta Webhook (Zapier)

### ¿Qué es un Webhook?

Los webhooks se utilizan normalmente para conectar dos aplicaciones diferentes. Cuando ocurre un evento en la aplicación de origen (disparador), esta serializa los datos de dicho evento y los envía a una URL de webhook de la aplicación de destino, que es la que realizará una acción basada en los datos recibidos. La aplicación de destino puede, entonces, enviar un mensaje de confirmación (callback).

Dicho de otro modo, al utilizar un webhook, todos los datos proporcionados por la primera aplicación se enviarán automáticamente a una segunda aplicación. Una vez que los datos llegan a la segunda aplicación, usted puede definir qué cantidad de esos datos se utilizará, cómo y dónde se colocarán, creando así una gestión de datos totalmente personalizada.

En esta solución, utilizaremos un caso en el que deseamos recopilar datos relacionados con un evento de Anuncio Entregado (Ad-Delivered). De todos los datos recolectados de ese evento, utilizaremos únicamente la **Marca de Tiempo** (Time Stamp), el **Dominio**, el **ID de la Campaña** y el **ID del Anuncio**. Una vez que obtengamos esos datos, crearemos una acción para enviarlos a una hoja de cálculo de Google (Google Sheet).

La razón principal para recopilar esos datos específicos es que queremos conocer el dominio exacto donde el usuario recibe nuestros banners y verificar si estos dominios son relevantes para el público objetivo de nuestra campaña.

### Requisitos

* Pipeline de Eventos u otra función que utilice Webhook.
* Zapier o cualquier herramienta que tenga una función Webhook.
* Hojas de cálculo de Google.
* Active Campaign.

Siga los pasos que se indican a continuación para gestionar correctamente sus datos a través de un webhook.

* [Creación de una Pipeline de Eventos](webhook-tool-zapier.md#creating-an-event-pipe)
* [Configuración de la herramienta de Webhook](webhook-tool-zapier.md#configuring-your-webhook-tool) (Zapier)
* [Activador](webhook-tool-zapier.md#trigger)
* [Acción](webhook-tool-zapier.md#action)
* [¡Comienza a recopilar Datos!](webhook-tool-zapier.md#start-collecting-data)

### Creación de Pipeline de Eventos

Para utilizar un webhook, utilizaremos la función Pipeline de Eventos para recopilar datos de una campaña en curso.

Cuando utilices el **Webhook de Zapier**, ve a la [Activador](webhook-tool-zapier.md#trigger) primero, sigue los pasos para obtener el enlace Webhook y completar la configuración de tu canal de eventos.

Vaya a nuestra pestaña Supervisión y haga clic en **Pipeline de Eventos.**

<div align="center"><figure><img src="../.gitbook/assets/image (491).png" alt=""><figcaption><p>Pestaña Supervisión</p></figcaption></figure></div>

Allí, crearemos un canal de eventos haciendo clic en <img src="../.gitbook/assets/image (492) (1).png" alt="Create Event Pipe" data-size="line">, en este caso, crearemos un evento ADS - Entregado, por lo que seleccionaremos la plantilla de evento de muestra, nuestra plantilla ADS - Entregado.

<figure><img src="../.gitbook/assets/image (407).png" alt="" width="538"><figcaption><p>Pantalla de Pipeline de Eventos</p></figcaption></figure>

A continuación, haga clic en <img src="../.gitbook/assets/image (494) (1).png" alt="Add Filter" data-size="line"> para añadir un filtro para recopilar datos de eventos relacionados con la entrega de anuncios, buscando eventos que contengan "entrega de anuncios" en su campo Tipo.

<figure><img src="../.gitbook/assets/image (496) (1).png" alt="" width="529"><figcaption><p>Filtro de Pipeline de Eventos</p></figcaption></figure>

Ve a la pestaña Destinos, ahí es donde configuramos nuestro enlace webhook, haz clic en <img src="../.gitbook/assets/image (498).png" alt="Add Target" data-size="line"> y luego selecciona Llamar a Webhook.

<figure><img src="../.gitbook/assets/image (499).png" alt="" width="543"><figcaption><p>Crear pantalla de destino</p></figcaption></figure>

Inserte la URL proporcionada por Zapier o su herramienta de gestión de datos y, a continuación, **guarde** su Objetivo y Pipeline de Eventos.

{% hint style="warning" %}
En algunas herramientas es **posible** que ya tengas disponible el enlace del Webhook. Si utilizas **Zapier**, primero tendrás que configurar tu webhook para obtener el enlace.
{% endhint %}

<figure><img src="../.gitbook/assets/image (637).png" alt="" width="542"><figcaption><p>Zapier Webhook configurado</p></figcaption></figure>

Asegúrate de tener habilitado tu Pipeline de Eventos y una campaña activa para recopilar datos y enviarlos a tu herramienta webhook.

<figure><img src="../.gitbook/assets/image (638).png" alt=""><figcaption><p>Pestaña Pipeline de Eventos habilitada</p></figcaption></figure>

### Configuración de la herramienta Webhook

Para esta solución utilizaremos Zapier como ejemplo, pero puedes utilizar tu herramienta de gestión de datos favorita, el único requisito es que tenga la función Webhook.

Zapier es una herramienta que presenta múltiples integraciones que pueden promover la automatización de tus tareas diarias. Es una herramienta de pago que tiene una versión de prueba en la que puedes comprobar si te resulta útil. Tendrás que crear una cuenta para empezar a utilizarla, incluso durante el periodo de prueba.

Si también vas a utilizar Zapier, este es el enlace para acceder: [Zapier](https://zapier.com).

En Zapier, haz clic en <img src="../.gitbook/assets/image (184).png" alt="Create" data-size="line">, y luego Zaps.

<figure><img src="../.gitbook/assets/image (501).png" alt="" width="221"><figcaption><p>Menú de creación de Zapier</p></figcaption></figure>

A continuación, configuraremos nuestro disparador y nuestra acción, basándonos en Webhook + Pipeline de Eventos + Google Sheets.

<figure><img src="../.gitbook/assets/image (502).png" alt="" width="489"><figcaption><p>Desencadenante y acción de Zapier</p></figcaption></figure>

### Gatillo

Este es el paso más importante, ya que aquí obtendrá la URL del webhook para comenzar a recopilar datos del BMS.

Para configurar nuestro disparador, haz clic en Disparador y luego en Buscar webhooks de Zapier.

<figure><img src="../.gitbook/assets/image (417).png" alt=""><figcaption><p>Función Webhook</p></figcaption></figure>

A continuación, ve a la pestaña App & Event (Aplicación y evento) situada a la derecha, donde podrás configurar tu evento como un evento Catch Hook.

<figure><img src="../.gitbook/assets/image (504) (1).png" alt="" width="404"><figcaption><p>Configuración de Webhooks</p></figcaption></figure>

Ve a la pestaña Prueba y obtén tu **URL de Webhook.**

Esta URL se utilizará en la configuración de Pipeline de Eventos [aquí](webhook-tool-zapier.md#creating-an-event-pipe).

<figure><img src="../.gitbook/assets/image (506).png" alt="" width="410"><figcaption><p>URL del Webhook</p></figcaption></figure>

Después de configurar la URL del webhook en tu Pipeline de Eventos, haz clic en "Test Trigger" (Probar activador) para recopilar una muestra de datos y utilizarla para configurar tu Google Sheet.

{% hint style="warning" %}
_¡Atención! Asegúrate de tener una campaña **activa** y de que tu canal de eventos esté **habilitado** para disponer de datos para esa prueba. Ten en cuenta que la prueba es **necesaria** para que haya datos disponibles para la configuración posterior en el paso de acción._
{% endhint %}

Los datos pueden tardar un tiempo en estar disponibles, una vez que su Pipeline de Eventos envíe la información a su herramienta, estos serán los datos que obtendrá de ese evento.

<figure><img src="../.gitbook/assets/image (639).png" alt="" width="402"><figcaption><p>Datos recopilados por Zapier</p></figcaption></figure>

Haga clic en <img src="../.gitbook/assets/image (935).png" alt="" data-size="line"> y luego pasaremos a configurar la acción que se llevará a cabo después de recopilar los datos.

Si se han seguido correctamente todos los pasos, su Gatilho tendrá un <img src="../.gitbook/assets/image (937).png" alt="Check" data-size="line"> informando de que funciona según lo previsto.

### Acción

Utilizaremos **Google Sheets** para gestionar los datos recopilados.

<figure><img src="../.gitbook/assets/image (936).png" alt="" width="377"><figcaption><p>Desencadenante y acción</p></figcaption></figure>

Crear un Google sheet en tu cuenta preferida y, a continuación, prepara las columnas para configurarlas.

En este ejemplo, recopilaremos los siguientes datos: **marca de** **tiempo**, **dominio**, **ID de campaña** e **ID de anuncio**.

Ten en cuenta que puedes nombrar tus columnas según tus necesidades, siéntete libre de establecer cualquier identificación que te resulte más adecuada.

<figure><img src="../.gitbook/assets/image (938).png" alt="" width="333"><figcaption><p>Google Sheet Configurado</p></figcaption></figure>

Utilizaremos el evento Crear fila en hoja de cálculo en nuestro Google sheet configuración de la acción.

<figure><img src="../.gitbook/assets/image (939).png" alt="" width="410"><figcaption><p>Configuración de eventos de acción</p></figcaption></figure>

Después de configurar tu cuenta en la pestaña Cuenta, ve a la pestaña Acción.

Allí configuraremos nuestra hoja de cálculo, la hoja de trabajo y qué datos se enviarán a cada columna.

<figure><img src="../.gitbook/assets/image (854).png" alt="" width="408"><figcaption><p>Hoja de cálculo y hoja de trabajo configuradas</p></figcaption></figure>

Para buscar mejor cada valor, escriba en la pestaña de búsqueda el valor que desea recopilar.

<figure><img src="../.gitbook/assets/image (855).png" alt=""><figcaption><p>Recopilación de datos</p></figcaption></figure>

Después de configurar todos los campos de datos con la muestra recopilada de la prueba de activación, estará listo para comenzar la prueba.

<figure><img src="../.gitbook/assets/image (942).png" alt="" width="400"><figcaption><p>Prueba de acción</p></figcaption></figure>

Haga clic en <img src="../.gitbook/assets/image (857).png" alt="" data-size="line"> y confirme que los datos se han enviado a su Spreadsheet.

<figure><img src="../.gitbook/assets/image (404).png" alt="" width="563"><figcaption><p>Datos enviados a Spreadsheet</p></figcaption></figure>

Si se han seguido correctamente todos los pasos, sus eventos tendrán un <img src="../.gitbook/assets/image (859).png" alt="Check" data-size="line">.

<figure><img src="../.gitbook/assets/image (860).png" alt="" width="251"><figcaption><p>Eventos verificados</p></figcaption></figure>

Haga clic en <img src="../.gitbook/assets/image (861).png" alt="" data-size="line"> para habilitar tu Webhook, todos los datos que se envían desde nuestra función Pipeline de Eventos estarán disponibles en tu Google Sheets!

### ¡Empieza a recopilar datos!

Una vez que tengas una campaña activa, Pipeline de Eventos y Webhook, así es como tu Google Sheet se actualizará.

<figure><img src="../.gitbook/assets/Spreadsheetdata Animated.gif" alt="" width="563"><figcaption><p>Actualización en tiempo real de Google Sheet</p></figcaption></figure>

{% hint style="info" %}
_Si te interesa obtener más información sobre los webhooks a través de Zapier, aquí encontrarás información más detallada:_ [_Guía de Webhooks de Zapier_](https://zapier.com/blog/what-are-webhooks/)
{% endhint %}

{% hint style="info" %}
_Hay muchas herramientas que se pueden utilizar para configurar un Webhook, así que busca la que mejor se adapte a tus necesidades. Zapier es solo una de las muchas opciones disponibles._
{% endhint %}
