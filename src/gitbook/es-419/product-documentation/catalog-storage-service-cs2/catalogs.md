# Catálogos

En la pestaña Catálogos, podrá crear un catálogo y, a continuación, instalar un píxel en su página para que BMS pueda recopilar datos de su página basándose en los siguientes eventos:

* Producto visto
* Producto añadido al carrito
* Producto pedido

Al añadir esos eventos a tu página, podremos recopilar todos los datos necesarios para empezar a crear métricas y, a continuación, utilizar nuestros **Modelos de Recomendación** para mejorar tus anuncios.

## **Gestión de Catálogos**

### Creación de un Catálogo

Para crear un catálogo, haga clic en <img src="../../.gitbook/assets/image (20).png" alt="Create Catalog" data-size="line"> botón.

<figure><img src="../../.gitbook/assets/image (21).png" alt="" width="539"><figcaption><p>Crear pantalla de catálogo</p></figcaption></figure>

Elige un **nombre** para tu catálogo y, si lo deseas, añade **etiquetas** para identificarlo mejor.

Después de rellenar los campos, haga clic en <img src="../../.gitbook/assets/image (22).png" alt="Save" data-size="line">.

Entonces tu catálogo estará disponible en tu lista.

<figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption><p>Lista del Catálogo</p></figcaption></figure>

### Edición de un Catálogo

Si necesita editar el nombre o las etiquetas de un catálogo, haga clic en <img src="../../.gitbook/assets/image (24).png" alt="Edit" data-size="line">, después de realizar los cambios necesarios, haga clic en <img src="../../.gitbook/assets/image (25).png" alt="Save" data-size="line">.

### Archivar un Catálogo

Para archivar un catálogo, haga clic en <img src="../../.gitbook/assets/image (26).png" alt="Archive" data-size="line">, a continuación, su catálogo archivado aparecerá en la lista Archivado. Para cambiar la vista, active el botón. <img src="../../.gitbook/assets/image (27).png" alt="Toggle" data-size="line">.

### Desarchivar un Catálogo

Para desarchivar un catálogo, cambie la vista a la lista Archivado y haga clic en <img src="../../.gitbook/assets/image (28).png" alt="Unarchive" data-size="line">, y su catálogo volverá a los catálogos activos.

### Eliminación de un Catálogo

Para eliminar un catálogo, haga clic en <img src="../../.gitbook/assets/image (29).png" alt="Delete" data-size="line">, se mostrará una pantalla para confirmar la eliminación.

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption><p>Pantalla de eliminación del Catálogo</p></figcaption></figure>

Después de hacer clic en <img src="../../.gitbook/assets/image (31).png" alt="Delete" data-size="line">, tu catálogo se eliminará de forma **permanente**.

{% hint style="danger" %}
_¡Atención! Le recomendamos que desactive el Catálogo en lugar de eliminarlo por completo. Al eliminar un catálogo, también se pierden todos los datos y métricas._
{% endhint %}

## Instalación de Catálogos

Para activar nuestras métricas y eventos, es necesario que instales un píxel en tu sitio web para comenzar a recopilar datos.

Seleccione el Catálogo en el que desea instalar sus píxeles y, a continuación, vaya a la pestaña Instrucciones de instalación.

<figure><img src="../../.gitbook/assets/image (105).png" alt=""><figcaption><p>Pestaña Instrucciones de instalación</p></figcaption></figure>

Cada evento tiene una página correcta para instalar tu píxel. Consulta la descripción de cada evento para saber exactamente dónde.

{% hint style="info" %}
Recuerda sustituir el marcador de posición por tu ID de oferta. Cada sitio web tiene su propia forma de definir una variable de ID de oferta, así que presta atención a cómo se ha configurado esta variable en tu sitio web. Si no se utiliza la variable correcta para tus productos, **el evento no funcionará**. Asegúrate de que la variable de ID de oferta de tu sitio web devuelve los mismos valores que se importaron como identificadores de producto (en nuestra plataforma, se denominan ID de oferta) en tu catálogo.&#x20;
{% endhint %}

_**Ejemplo:** El evento Producto solicitado debe instalarse en la página de **confirma**_**ción del pedido**.

## Pestaña Métricas <a href="#metrics" id="metrics"></a>

Una vez que haya creado su catálogo e instalado correctamente sus píxeles, las métricas comenzarán a completarse y podrá realizar un seguimiento de los eventos a medida que se produzcan.

Hay disponible una amplia lista de métricas y es posible agruparlas por **catálogo**, **canal de importación** y **modelo de recomendación**, cada uno con sus propias métricas. También puede seleccionar varios catálogos para compararlos y evaluar su rendimiento.

Estas son todas las métricas disponibles para la función Catálogos:

* [Recuento de trabajos de importación](cs2-metrics.md#import-job-count)
* [Duración del trabajo de importación](cs2-metrics.md#import-job-duration)
* [Tasa de errores del trabajo de importación](cs2-metrics.md#import-job-failure-rate)
* [Problemas del trabajo de importación](cs2-metrics.md#import-job-issues)
* [Bytes procesados ​​del trabajo de importación](cs2-metrics.md#import-job-processed-bytes)
* [Registros procesados ​​del trabajo de importación](cs2-metrics.md#import-job-processed-records)
* [Recuento de productos añadidos al carrito](cs2-metrics.md#product-added-to-cart-count)
* [Recuento de productos](cs2-metrics.md#product-count)
* [Recuento de pedidos de productos](cs2-metrics.md#product-order-count)
* [Recuento de recomendaciones de productos](cs2-metrics.md#product-recommendation-count)
* [Recuento de vistas de productos](cs2-metrics.md#product-view-count)
* [Productos añadidos](cs2-metrics.md#products-added)
* [Productos eliminados](cs2-metrics.md#products-removed)
* [Productos actualizados](cs2-metrics.md#products-updated)
* [Recuento de clics en recomendaciones](cs2-metrics.md#recommendation-click-count)
* [Tasa de cumplimiento de recomendaciones](cs2-metrics.md#recommendation-fulfillment-rate)
* [Recuento de vistas de recomendaciones](cs2-metrics.md#recommendation-view-count)
* [Recuento de solicitudes de recomendaciones](cs2-metrics.md#recommendation-request-count)
