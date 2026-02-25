---
description: Más información sobre los modelos de recomendación y cómo crearlos.
---

# Modelos de Recomendación

Utiliza modelos de recomendación para mostrar tus productos en banners dinámicos, que muestran diferentes productos según quién recibe el anuncio, con el objetivo de aumentar tus conversiones.

## Gestión de Modelos de Recomendación

<figure><img src="../../.gitbook/assets/image (62) (1).png" alt=""><figcaption><p>Lista de Modelos de Recomendación</p></figcaption></figure>

### Creación de Modelos de Recomendación

Antes de crear un modelo de recomendación, es necesario configurar los catálogos y los servicios DMP que actuarán como fuentes para nuestros modelos de recomendación.

1. Haga clic en <img src="../../.gitbook/assets/image (254).png" alt="" data-size="line"> para empezar a crear un modelo de recomendación.
2.  Rellene los datos:

    <figure><img src="../../.gitbook/assets/image (264).png" alt=""><figcaption><p>Editor de modelos de recomendación</p></figcaption></figure>

    * Nombre: Introduzca un nombre para su modelo de recomendación.
    * Etiquetas: Establezca etiquetas para su organización.
    * Catálogo: Seleccione el catálogo que contiene los productos que utilizará para este modelo de recomendación.
3. Haga clic en <img src="../../.gitbook/assets/image (256).png" alt="" data-size="line"> para guardar tu modelo de recomendación.

### Configuración de Modelos de Recomendación

Después de crear un modelo de recomendación, es necesario configurar sus fuentes antes de poder utilizarlo. Esto se puede hacer en la pestaña de configuración:

<figure><img src="../../.gitbook/assets/Captura de tela 2024-05-15 095125.png" alt=""><figcaption><p>Pestaña Configuración de modelos de recomendación</p></figcaption></figure>

1. Seleccione un modelo de recomendación de la lista.
2. Haga clic en <img src="../../.gitbook/assets/image (56) (1).png" alt="" data-size="line"> para añadir una fuente para este modelo.
3.  Rellene los datos:

    <figure><img src="../../.gitbook/assets/image (50) (2).png" alt=""><figcaption><p>Editor de fuentes de modelos de recomendación - Rastreador DMP</p></figcaption></figure>

    * Nombre: Indique un nombre para su fuente.
    * Límite: Establezca el número máximo de productos que se añadirán al modelo de recomendación por esta fuente.
    * Tipo: Seleccione el tipo de fuente que desea utilizar:
      1. DMP Rastreador: esta opción añadirá productos al modelo de recomendación basándose en los datos de actividad recopilados en su sitio web.
         * Rastreador: Seleccione el rastreador que desea utilizar.
         * Evento de Rastreador: seleccione el evento seguido que se tendrá en cuenta para añadir productos al modelo de recomendación.
         * Campo que contiene los ID de las ofertas: Indique el campo personalizado que contiene el ID de las ofertas de los productos que desea incluir en este modelo de recomendación.
         * Plantilla: Especifique una plantilla para generar una lista de ID de ofertas separadas por comas para realizar el seguimiento.
      2.  Clasificación de productos CS2: Esta opción añadirá productos al modelo de recomendación basándose en la actividad recopilada por su catálogo de productos.

          <figure><img src="../../.gitbook/assets/image (253).png" alt=""><figcaption><p>Editor de fuentes de modelos de recomendación - Clasificación de productos CS2</p></figcaption></figure>

          * Clasificar por: Seleccione una actividad clasificada entre las opciones disponibles:
            * Más añadidos al carrito: Esta opción añadirá los productos más añadidos al carrito a tu modelo de recomendación.
            * Más solicitados: Esta opción añadirá los productos más solicitados a su modelo de recomendación.
            * Recomendación más clicada: Esta opción solo se puede utilizar después de ejecutar una campaña con modelos de recomendación, y llenará su modelo de recomendación con los productos que se recomendaron anteriormente y en los que ha hecho clic un usuario.
            * Recomendaciones más vistas: Esta opción solo se puede utilizar después de ejecutar una campaña con modelos de recomendación, y llenará su modelo de recomendación con los productos que se recomendaron anteriormente y que han sido vistos por un usuario.
            * Más recomendados: Esta opción solo se puede utilizar después de ejecutar una campaña con modelos de recomendación y llenará su modelo de recomendación con los productos más recomendados.
            * Más vistos: Esta opción añadirá los productos más vistos a tu modelo de recomendación.
          * En las últimas horas: Establezca un número de horas en el pasado para tener en cuenta la actividad recopilada durante ese periodo a la hora de añadir productos al modelo de recomendación.
4. Haga clic en <img src="../../.gitbook/assets/image (256).png" alt="" data-size="line"> para guardar tu fuente.

Inmediatamente después de crear tu fuente, estará disponible una vista previa de tus productos recomendados. Para que se genere esta vista previa, debes tener instalados en tu sitio web tus grupos de cookies y rastreadores y/o tus eventos de catálogo, ya que sus datos se utilizarán para generar las recomendaciones.

<figure><img src="../../.gitbook/assets/image (64) (1).png" alt=""><figcaption><p>Pestaña Configuración de modelos de recomendación: Vista Previa.</p></figcaption></figure>

### Modelos y Fuentes de Recomendaciones de Edición

Hay algunas opciones de edición disponibles para los modelos y fuentes de recomendación.

#### Modelos de Recomendación

Puede editar el nombre y las etiquetas de un modelo de recomendación, sin embargo, el catálogo no se puede cambiar. Para realizar esta edición, haga clic en <img src="../../.gitbook/assets/image (115).png" alt="" data-size="line"> en la misma fila que el modelo de recomendación que se va a editar.

#### Fuentes

Todos los detalles de la fuente son editables, seleccione el modelo de recomendación que contiene la fuente que desea editar. A continuación, en la pestaña de configuración, en la sección de fuentes, haga clic en <img src="../../.gitbook/assets/image (115).png" alt="" data-size="line"> igual que la fuente que se va a editar, realice los cambios y, a continuación, haga clic en <img src="../../.gitbook/assets/image (256).png" alt="" data-size="line"> para guardarlos. También puedes duplicar una fuente haciendo clic en <img src="../../.gitbook/assets/image (401).png" alt="" data-size="line">. Esto resulta útil si necesitas otra fuente con solo unos pocos cambios respecto a una ya existente, pero sin eliminar esta última.

### ¿Cómo funcionan las Fuentes?

Las fuentes son la forma en que recopila datos para alimentar su modelo de recomendación. El modelo de recomendación necesita estos datos para organizar los productos según lo previsto. Debe elegir entre un rastreador DMP o una clasificación de productos CS2; ambos métodos funcionan bien, pero cada uno requiere pasos adicionales para una configuración adecuada. Una vez que haya configurado correctamente su fuente, su modelo de recomendación comenzará a recopilar datos y a actualizarse activamente, proporcionando a su anuncio la información más actualizada.&#x20;

### Eliminación de Modelos y Fuentes de Recomendación

{% hint style="danger" %}
¡Atención! Tenga cuidado al eliminar modelos de recomendación, ya que esta acción no se puede deshacer y todos los datos relacionados, incluidas las métricas recopiladas anteriormente, también se eliminarán.
{% endhint %}

Puede archivar un modelo de recomendación haciendo clic en <img src="../../.gitbook/assets/image (63) (1).png" alt="" data-size="line"> en la misma fila que el modelo de recomendación que necesitamos archivar. También es posible eliminar un modelo de recomendación, sin embargo, esto eliminará todas las métricas relacionadas con él, esta acción no se puede deshacer, así que ten cuidado al realizarla. Haz clic en <img src="../../.gitbook/assets/image (402).png" alt="" data-size="original"> en la misma fila que el modelo de recomendación que se va a eliminar. A continuación, confirme la acción haciendo clic en <img src="../../.gitbook/assets/image (403).png" alt="" data-size="line">. Esta acción no se puede deshacer.

Es posible eliminar una fuente. Sin embargo, esto también eliminará todas las métricas relacionadas con esta fuente, por lo que debe tener cuidado al realizar esta acción. En la sección de fuentes de la pestaña de configuración, haga clic en <img src="../../.gitbook/assets/image (402).png" alt="" data-size="original"> en la misma fila que la fuente que se va a eliminar. A continuación, confirme la acción haciendo clic en <img src="../../.gitbook/assets/image (403).png" alt="" data-size="line">. Esta acción no se puede deshacer.

## Pestaña Métricas

Después de configurar sus modelos de recomendación y comenzar a utilizarlos para una campaña, debería empezar a recibir datos de ellos. Es posible seguir este proceso en la pestaña de métricas. Estas son las métricas disponibles para los modelos de recomendación:

* [Recuento de recomendaciones de productos](cs2-metrics.md#product-recommendation-count)
* [Recuento de clics en recomendaciones](cs2-metrics.md#recommendation-click-count)
* [Tasa de cumplimiento de recomendaciones](cs2-metrics.md#recommendation-fulfillment-rate)
* [Recuento de solicitudes de recomendaciones](cs2-metrics.md#recommendation-request-count)
* [Recuento de visualizaciones de recomendaciones](cs2-metrics.md#recommendation-view-count)
