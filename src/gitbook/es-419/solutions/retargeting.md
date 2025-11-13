# Creación de una Campaña de Retargeting

El retargeting es una estrategia de publicidad en línea diseñada para volver a atraer a los usuarios que anteriormente visitaron su sitio web o aplicación móvil, pero no completaron una acción deseada, como comprar un producto, registrarse o llenar un formulario.

El objetivo principal del retargeting es traer de vuelta a estos usuarios a su sitio o aplicación y motivarlos a completar la acción que inicialmente pretendían realizar.

Para ayudarle a crear una campaña de retargeting de principio a fin, hemos desarrollado este artículo. A continuación, verá los temas que abordaremos con este propósito:

* [Creación e instalación de un **Cookie Pool**](retargeting.md#creating-a-cookie-pool)
* [Creación de un **Catálogo** e **Import Channels**](retargeting.md#creating-a-catalog)
* [Creación, configuración e instalación de un **Tracker**](retargeting.md#creating-trackers)
* [Creación de **Modelos de Recomendación**](retargeting.md#creating-a-recommendation-model)
* [Uso del **Creative Builder** para crear **Builds** y **Blueprints**](retargeting.md#creative-builder)
* [Creación de **Grupos de Creativos**](retargeting.md#creating-a-creative-group)
* [Creación de **Anuncios** y **Bulk Ads**](retargeting.md#creating-an-a-d)
* [Configuración de **Reglas para Anuncios**](retargeting.md#creating-a-rule)
* [Creación de una **Campaña de Retargeting**](retargeting.md#creating-a-campaign)

## Cookie Pool

Comenzamos creando e instalando un **Cookie Pool** en su sitio web. Un cookie pool es una base de datos construida a partir de las cookies almacenadas de los usuarios. Las cookies son pequeños archivos guardados en el navegador web de un usuario que contienen datos sobre su comportamiento en internet.

La función de cookie pool recopila información adicional sobre la segmentación de la audiencia y mejora el rendimiento de la campaña.

### Creación de un Cookie Pool

1. En la [página principal de BMS](https://console.bluems.com/), en la sección DMP, haga clic en Cookie Pools.
2. Haga clic en <img src="../.gitbook/assets/image (335).png" alt="+ cookie pool button" data-size="line"> para crear un Cookie Pool.
3. Ahora puede asignarle un Nombre y Etiquetas.
4. Inserte su dominio y seleccione los exchanges que desee.
5. Establezca el período y el tamaño del cookie pool.
6. Haga clic en <img src="../.gitbook/assets/image (331).png" alt="Save Button" data-size="line"> para guardar su cookie pool.

### Instalación de un Cookie Pool

1. En la [página de Cookie Pools](https://console.bluems.com/dmp/cookie-pools), seleccione la pestaña install instructions.
2. Haga clic en <img src="../.gitbook/assets/image (336).png" alt="Copy button" data-size="line"> para copiar la etiqueta del cookie pool.
3. Agregue este código en la etiqueta \<head> de las páginas donde desea que los usuarios sean añadidos al pool.
   * Recomendamos que esta acción la realice el desarrollador de su sitio web.
   * Alternativamente, puede instalar esta etiqueta en su sitio utilizando Google Tag Manager (GTM).

## Servicio de Almacenamiento de Catálogos (CS2)

Si desea promocionar productos de su sitio web en sus banners publicitarios, utilice el catálogo. Si este no es su objetivo, puede omitir este paso y continuar con la configuración de sus [rastreadores](retargeting.md#trackers).

Una vez que haya creado un conjunto de cookies, es momento de crear su catálogo de productos. Esto le permitirá utilizar modelos de recomendación que aumentan las conversiones de los anuncios al mostrar sus productos en banners dinámicos.

### Creación de un Catálogo

1. En la [página principal de BMS](https://console.bluems.com/), haga clic en Catalogs, en la sección CS2.
2. Haga clic en <img src="../.gitbook/assets/image (337).png" alt="Create Catalog Button" data-size="line"> para crear un nuevo catálogo.
3. Asigne un Nombre y Etiquetas.
4. Haga clic en <img src="../.gitbook/assets/image (333).png" alt="Save Button" data-size="line"> para guardar sus cambios.
5. Siga las instrucciones de la pestaña install instructions para instalar el píxel del catálogo en su sitio web:
   * En la pestaña install instructions, tendrá acceso a etiquetas de imagen, necesarias para rastrear las interacciones en su sitio web con los productos de su catálogo; cada etiqueta rastrea diferentes acciones en su sitio.
   * También es necesario reemplazar el marcador de posición indicado con su ID de oferta, el mismo ID que usa para importarlo, de modo que las métricas puedan sincronizarse.

{% hint style="danger" %}
¡Atención! Debe instalarlas con mucho cuidado en las páginas correctas para asegurarse de que solo se rendericen una vez por evento, ya que para la plataforma cada render se cuenta como un evento.
{% endhint %}

### Creación de un Import Channel

1. En el menú de la derecha, haga clic en Import Channels.
2. Haga clic en <img src="../.gitbook/assets/image (338).png" alt="+ import channel button" data-size="line"> para comenzar.
3. Aquí necesitamos configurar las tres pestañas disponibles para que funcione correctamente.

* Pestaña General
  1. Asigne un nombre y etiquetas a su Import Channel.
  2. Seleccione el catálogo desde el cual importará los datos de sus productos.
  3. Seleccione con qué frecuencia se debe actualizar su catálogo para agregar o editar sus productos.
  4. Seleccione con qué frecuencia se deben eliminar los productos de su catálogo.
* Pestaña Source
  1. Seleccione el protocolo utilizado en la URL desde la cual se importarán los productos.
  2. Ingrese la URL desde la cual se importarán los productos.
  3. Seleccione el formato de su catálogo entre las opciones disponibles.
* Pestaña Mapping
  1. Indique el modelo de plantilla de su catálogo; este paso puede requerir la ayuda de nuestro equipo técnico.
  2. Haga clic en <img src="../.gitbook/assets/image (334).png" alt="Save Button" data-size="line"> para guardar sus cambios.

Después de completar los pasos anteriores, active el Import Channel para comenzar a trabajar con él. También puede realizar una prueba para confirmar que funciona correctamente; para realizar esta prueba, siga los pasos a continuación:

1. Seleccione el Import Channel que desea probar.
2. Haga clic en <img src="../.gitbook/assets/image (339).png" alt=" Start Button" data-size="line"> para iniciar una importación manual.
3. Marque la opción 'Testing Mode'.
4. Seleccione cuántos productos se deben probar.
5. Configure si desea usar la configuración del canal para eliminar productos o si desea eliminarlos antes de que comience la prueba.
6. Haga clic en <img src="../.gitbook/assets/image (340).png" alt="Start Button" data-size="line"> para iniciar.
7. Seleccione el Import Channel que ha probado y, en la pestaña de jobs, puede confirmar si el canal funciona correctamente; en caso de problemas, estos se mostrarán en la columna "Issues".

### Productos

En esta sección, podrá ver todos sus productos. Marque la casilla de los productos y vaya a la pestaña de detalles para ver información más detallada, como el offer ID, por ejemplo.

## Rastreadores

Rastree las actividades en el sitio web de su audiencia usando trackers y utilice estos datos para crear un modelo de recomendación de productos basado en su catálogo.

### Creación de Trackers

1. En la [página principal de BMS](https://console.bluems.com/), haga clic en **Trackers**.
2. Haga clic en <img src="../.gitbook/assets/image (341).png" alt="+ tracker button" data-size="line"> para agregar un nuevo tracker.
3. Asigne un nombre a su tracker.
4. Configurar etiquetas le ayudará a encontrar este tracker más fácilmente.
5. Establezca el número máximo de usuarios. No se podrán agregar usuarios nuevos una vez alcanzado el límite, pero las acciones de los usuarios existentes seguirán siendo rastreadas.
6. Establezca la cantidad máxima de eventos rastreados por usuario; una vez alcanzado el límite, el sistema eliminará automáticamente los eventos más antiguos para dar espacio a los nuevos.
7. Configure cuánto tiempo desea utilizar estos trackers; después de este período, las actividades del tracker se eliminarán.

### Configuración de Rastreadores

Configura eventos para rastrear acciones específicas de tu audiencia.

1. En la [página de Rastreadores](https://console.bluems.com/dmp/trackers), selecciona un rastreador.
2. En la pestaña de configuración, haz clic en <img src="../.gitbook/assets/image (342).png" alt="Add button" data-size="line"> para crear un evento.
3. Asignar un nombre al evento generará automáticamente un ID para él.
4. Configura el campo de datos personalizados con la información que deseas rastrear, por ejemplo: "offerid".
5. Haz clic en <img src="../.gitbook/assets/image (343).png" alt="Add button" data-size="line"> para crear una acción que se ejecutará después de que el evento haya sido rastreado.
6. Asigna un nombre a la acción.
7. Elige entre una acción 'Call a Webhook' o 'Track in Catalog':
   * Para 'Call a Webhook', indica la URL a la que se deben enviar los datos. También puedes elegir actividades predeterminadas o personalizadas para rastrear.
   * Para 'Track in Catalog', selecciona el catálogo deseado y la actividad que deseas rastrear; también es posible rastrear actividades personalizadas.
8. Haz clic en <img src="../.gitbook/assets/image (344).png" alt="Save button" data-size="line"> para guardar la acción creada.
9. Puedes añadir más acciones a este evento y luego hacer clic nuevamente en <img src="../.gitbook/assets/image (345).png" alt="Save button" data-size="line"> para guardar el evento completo.

### Instalación de un Tracker en tu Sitio Web

Después de crear tus trackers, eventos y acciones, debes instalarlos en tu sitio web para comenzar a usarlos. Hay 3 métodos de instalación disponibles: Script, Pixel y Redirect.

**Script**

1. En la [página de rastreadores](https://console.bluems.com/dmp/trackers), selecciona el rastreador deseado.
2. Haz clic en la pestaña 'Install Instructions' y elige el evento que quieres rastrear.
3. Selecciona la opción Script.
4. Si configuraste campos de datos personalizados, usa los placeholders indicados para informar los valores.\
   Aquí tienes un ejemplo de cómo podría verse el placeholder indicado para tus campos de datos personalizados: <img src="../.gitbook/assets/image (347).png" alt=" Custom data field example" data-size="original">.\
   &#xNAN;_**Ejemplo:**_ Necesitas rastrear de qué color de producto están más interesados tus usuarios; podrás usar este campo para recopilar datos sobre el color del producto.
5. Haz clic en <img src="../.gitbook/assets/image (348).png" alt="copy button" data-size="line"> para copiar el script.
6. Añade este script al código de tu sitio web, en la página donde se rastreará el evento.
7. También puedes usar un tag manager, como Google Tag Manager, para añadir este script a tu sitio web.

**Pixel**

1. Después de elegir un evento en la pestaña 'Install Instructions', selecciona la opción Pixel.
2. Si configuraste campos de datos personalizados, usa los placeholders indicados para informar los valores.
3. Haz clic en <img src="../.gitbook/assets/image (348).png" alt="copy button" data-size="line"> para copiar la etiqueta Pixel.
4. Añade la etiqueta Pixel al código de tu sitio web, en la página donde se rastreará el evento.
5. También puedes usar un tag manager, como Google Tag Manager, para añadir esta etiqueta a tu sitio web.

**Redirect**

1. Después de elegir un evento en la pestaña 'Install Instructions', selecciona la opción Redirect.
2. Proporciona la URL a la que el usuario será redirigido después de que el evento sea capturado.
3. Si configuraste campos de datos personalizados, usa los placeholders indicados para informar los valores.
4. Haz clic en <img src="../.gitbook/assets/image (348).png" alt="copy button" data-size="line"> para copiar la URL generada y úsala como la URL proporcionada anteriormente.

### Pestaña de Métricas del Tracker

La pestaña de métricas permite visualizar cómo están funcionando tus trackers, eventos y acciones. En la pestaña de métricas de la página de rastreadores, es posible filtrar los datos mostrados según tu preferencia. Los filtros disponibles actualmente son:

* "Group By": Selecciona cómo deseas agrupar los datos mostrados, por tracker o por evento.
* "Visualization": Selecciona cómo deseas mostrar tus datos, tarjetas de métricas o tabla.
* "Period": Selecciona el periodo que contiene los datos que necesitas.

Los datos recolectados por los trackers permiten mostrar anuncios dinámicos y personalizados a tu público objetivo; sin ellos, es imposible generar o mostrar banners dinámicos.

## Modelos de Recomendación

Los modelos de recomendación se utilizan para llenar tus banners dinámicos con datos sobre tus productos, basándose en tus catálogos y en la actividad rastreada de tu sitio web.

### Crear un Modelo de Recomendación

1. En la [página principal de BMS](https://console.bluems.com/), haz clic en Modelos de Recomendación, en la sección CS2.
2. Haz clic en <img src="../.gitbook/assets/image (349).png" alt="Create recommendation model button " data-size="line"> para crear un nuevo modelo de recomendación.
3. Asigna un Nombre y Etiquetas.
4. Selecciona el catálogo del cual el modelo recopilará datos e interacciones de los leads.
5. Haz clic en <img src="../.gitbook/assets/image (350).png" alt="save button" data-size="line">para guardar los cambios.

Si dejas de usar un modelo de recomendación, se recomienda deshabilitarlo en lugar de eliminarlo, ya que al eliminar un modelo también se eliminan los datos recolectados por ese modelo.

### Configuración de una Fuente

Ahora que hemos creado nuestro modelo de recomendación, necesitamos configurar algunas fuentes para él. Hay 2 tipos de fuentes disponibles: Rastreadores DMP y Catálogos (CS2). Usar Rastreadores DMP como fuente relacionará tu modelo de recomendación con los datos recolectados por los rastreadores instalados en tu sitio web. La opción Catálogos (CS2) relacionará tu modelo de recomendación con los datos de tu catálogo, estableciendo un ranking de productos. A continuación se detallan los pasos para configurar una fuente según el tipo deseado:

* Rastreadores DMP
  1. Selecciona los modelos de recomendación que deseas usar con esta fuente.
  2. En la pestaña Configuración, haz clic en <img src="../.gitbook/assets/image (351).png" alt="+ add button" data-size="line"> para agregar una nueva Fuente.
  3. Asigna un Nombre.
  4. Establece un límite de productos del catálogo de los cuales se recopilarán datos.
  5. Elige Rastreador DMP como tipo de fuente.
  6. Selecciona el rastreador del cual recopilarás los datos.
  7. Selecciona el evento configurado en el rastreador del cual se recopilarán los datos.
  8. Establece el campo que contiene tus IDs de oferta.
  9. Haz clic en <img src="../.gitbook/assets/image (352).png" alt="save button" data-size="line"> para guardar los cambios.
* Ranking de Productos CS2
  1. Realiza los pasos 1-4 anteriores.
  2. Elige Ranking de Productos CS2.
  3. Selecciona la acción que deseas usar para rankear los productos de esta fuente.
  4. Indica el periodo durante el cual se revisarán y recopilarán las métricas.
  5. Haz clic en <img src="../.gitbook/assets/image (353).png" alt="save button" data-size="line"> para guardar los cambios.

Las fuentes se usan para llevar los datos de tus productos a tus banners dinámicos. Debes tener al menos una fuente por cada espacio disponible en tu banner dinámico, cada fuente llena solo un espacio a la vez; si tienes más espacios que fuentes, algunos espacios quedarán vacíos en tus banners dinámicos. También recomendamos configurar al menos 3 fuentes por modelo de recomendación.

## Constructor de Creativos

Usa el Constructor de Creativos para crear blueprints y builds que te ayudarán a generar tus anuncios más rápido.

### Blueprints

Los blueprints son modelos para crear anuncios de manera rápida y eficiente. Estos modelos predefinidos te permiten construir anuncios que satisfacen las necesidades de tu negocio con facilidad.

Construidos sobre lenguajes de diseño web, los blueprints te ofrecen la flexibilidad de crear banners dinámicos. Incluso si no estás familiarizado con los lenguajes de desarrollo web, puedes usar con confianza uno de los blueprints predefinidos disponibles.

#### Cómo usar Blueprints

Primero, deberás elegir entre crear un blueprint desde cero o usar un blueprint ya existente.

* **Creando un modelo de blueprint**
  1. Localiza y haz clic en Blueprints en la [página principal de BMS](https://console.bluems.com/).
  2. Haz clic en <img src="../.gitbook/assets/image (302).png" alt="add blueprint button" data-size="line">.
  3. Asigna un Nombre a tu Blueprint.
  4. Establece etiquetas para facilitar su búsqueda más adelante.
  5. Elige la disponibilidad según tu preferencia: seleccionar público hará que tu blueprint esté disponible para todos los usuarios de la plataforma BMS, y privado lo hará disponible solo para ti y aquellos con acceso a tu cuenta.
  6. Selecciona los tamaños de banner deseados.
  7. Haz clic en ![](<../.gitbook/assets/image (303).png>) para agregar un nuevo grupo de parámetros y comenzar a codificar tu banner.
  8. Puedes usar los parámetros del sistema según tus necesidades.
  9. También puedes usar nuestros Macros para mejorar la interacción con los usuarios de tus anuncios.
* **Usando un modelo de Blueprint existente**
  1. Localiza y haz clic en Blueprints en la [página principal de BMS](https://console.bluems.com/).
  2. Desactiva la opción 'Owned', esto mostrará todos los blueprints públicos disponibles en ese momento.
  3. Elige el blueprint según las necesidades de tu negocio entre las opciones disponibles.
  4. Haz clic en ![](<../.gitbook/assets/image (304).png>) para duplicar el blueprint a tu cuenta.
  5. Haz clic en ![](<../.gitbook/assets/image (305).png>) para comenzar a editar tu copia del blueprint; aquí puedes hacer cambios al blueprint, ajustándolo para reflejar mejor las necesidades de tu negocio.

### Builds

Crea builds usando tus modelos de blueprint; los builds te ayudan a crear banners dinámicos mostrando productos de tu catálogo, usados en tus campañas de retargeting.

#### Creando Banners Dinámicos Usando Builds

1. En la [página principal de BMS](https://console.bluems.com/), localiza y haz clic en Builds.
2. Haz clic en <img src="../.gitbook/assets/image (361).png" alt="create build button" data-size="line"> para comenzar a crear un nuevo build.
3. Asigna un Nombre, también puedes agregar etiquetas para facilitar su seguimiento.
4. Elige tu dominio.
5. Selecciona un modelo de blueprint.
6. Selecciona los tamaños de tus banners. Se recomienda usar tamaños con proporciones iguales para cada build; por ejemplo, usa un build para banners verticales y otro para banners horizontales, esto mantendrá las proporciones de los logos, imágenes y productos mostrados.
7. Usa los Parámetros en el lado izquierdo para configurar y personalizar tus logos, imágenes, grillas de productos y más.
8. Al cambiar los parámetros, podrás ver una vista previa en vivo de cómo se mostrará tu banner, ayudándote a encontrar el ajuste perfecto para las necesidades de tu negocio.
9. Marca la casilla "Enviar creativos para aprobación" y haz clic en <img src="../.gitbook/assets/image (362).png" alt="" data-size="line"> para guardar tu build y enviarlo a revisión de los Ad Exchanges.

## Grupos Creativos

Agrupa varios creativos como una unidad para aplicar diferentes pesos y comparar el rendimiento entre variantes; esta comparación se conoce como prueba A/B y es muy útil para descubrir qué tipos de creativos son más interesantes para tu audiencia.

### Creando un Grupo Creativo

1. En la [página principal de BMS](https://console.bluems.com/), haz clic en Creative Groups, en la sección AdServing.
2. Haz clic en <img src="../.gitbook/assets/image (363).png" alt="add creative build button" data-size="line"> para crear un nuevo grupo creativo.
3. Asigna un Nombre y Etiquetas.
4. Selecciona tu dominio.
5. Selecciona el formato de los creativos en el grupo.
6. Selecciona los creativos que deberían formar parte de este grupo. Haz clic en <img src="../.gitbook/assets/image (365).png" alt="Add button" data-size="line"> para agregar más campos y seleccionar tus creativos.
7. Establece un peso para cada creativo agregado.&#x20;
   * Este peso define qué creativos se mostrarán más frecuentemente a tu público objetivo; mientras mayor sea el peso de un creativo, más se mostrará.
8. Puedes obtener una vista previa de tu grupo al finalizar esta configuración; haz clic en <img src="../.gitbook/assets/image (364).png" alt="Preview group button" data-size="original"> para ver la vista previa.
9. Haz clic en <img src="../.gitbook/assets/image (362).png" alt="" data-size="line"> para guardar los cambios.

## Anuncios

Aquí es donde creas tus anuncios usando tus grupos creativos y los envías a revisión de los Ad Exchanges; también puedes crear reglas para controlar cómo se entregarán tus anuncios y seguir el estado y las métricas de los mismos.

### Creando un Anuncio

1. En la [página principal de BMS](https://console.bluems.com/), haz clic en Ads, en la sección AdServing.
2. Haz clic en <img src="../.gitbook/assets/image (367).png" alt="create add button" data-size="line"> para crear tu anuncio.
3. Asigna un Nombre y Etiquetas.
4. Selecciona tu dominio.
5. Elige un formato para tu anuncio.
6. Selecciona el grupo creativo que deseas usar.
7. Si no tienes un grupo creativo o necesitas uno nuevo, puedes crearlo rápidamente haciendo clic en <img src="../.gitbook/assets/image (368).png" alt="create a creative group button" data-size="original">.
8. Marca la casilla para enviar tu anuncio a revisión en todos los Ad Exchanges soportados.
9. Haz clic en <img src="../.gitbook/assets/image (362).png" alt="" data-size="line"> para guardar tu anuncio.

### Anuncios Masivos

Esta opción te permite crear anuncios de forma rápida y masiva.

1. Haz clic en <img src="../.gitbook/assets/image (370).png" alt="Create bulk ads button" data-size="line"> para comenzar.
2. Asigna un Nombre y Etiquetas para tus anuncios.
3. Selecciona tu dominio.
4. Indica la URL a la que debe redirigir el anuncio al hacer clic; se permite parametrización (por ejemplo, UTM).
5. Haz clic en <img src="../.gitbook/assets/image (354).png" alt="" data-size="line"> para agregar las imágenes de tus creativos según las siguientes opciones:
   * Usar Existentes
     1. Selecciona todas las imágenes que quieras entre las que ya has subido a la plataforma.
     2. Haz clic en <img src="../.gitbook/assets/image (355).png" alt="" data-size="line"> para confirmar tu selección.
   * Subir Nuevas
     1. Sube nuevas imágenes arrastrándolas a la caja o haciendo clic en <img src="../.gitbook/assets/image (356).png" alt="" data-size="line"> y seleccionándolas desde tu dispositivo.
     2. Haz clic en <img src="../.gitbook/assets/image (355).png" alt="" data-size="line"> para confirmar.
   * Usar Dirección Web (URL)
     1. Añade una URL por línea.
     2. Haz clic en <img src="../.gitbook/assets/image (355).png" alt="" data-size="line"> para confirmar.
6. Marca la opción de agrupar creativos del mismo formato para poder realizar una prueba A/B.
7. Marca la opción para enviar tus anuncios a revisión de los Ad Exchanges.
8. Haz clic en <img src="../.gitbook/assets/image (357).png" alt="" data-size="line"> para guardar tus anuncios y enviarlos a revisión.

### Reglas

En esta pestaña puedes configurar reglas para que tus anuncios se ejecuten solo en horarios y días específicos.

#### Creando una Regla

1. Selecciona el anuncio al que deseas configurar una regla.
2. En la pestaña Rules, haz clic en <img src="../.gitbook/assets/image (358).png" alt="" data-size="line"> para agregar una nueva regla.
3. Asigna un Nombre y selecciona qué Grupo Creativo debe verse afectado.
4. Activa la opción de Programación cambiando el interruptor a “on” <img src="../.gitbook/assets/image (359).png" alt="" data-size="original"> .
5. Selecciona las horas en las que deseas que tus anuncios se muestren cada día. Si hay días en los que no quieres que se ejecute el anuncio, desmarca todas las horas de esos días y no se mostrará en ellos.
6. Haz clic en <img src="../.gitbook/assets/image (360).png" alt="" data-size="line"> para guardar tu regla.
7. Las reglas pueden activarse o desactivarse en cualquier momento, simplemente cambiando entre “on” y “off” en la pestaña de reglas.

### Revisiones de Ad Exchange

En la pestaña Exchange Reviews, después de crear tu anuncio, selecciónalo para monitorear si los Ad Exchanges lo aprueban o rechazan. En caso de rechazo, puedes verificar el motivo en la columna de comentarios. Luego de realizar los ajustes necesarios, podrás reenviar el anuncio para una nueva revisión.

## Campañas

Aquí encontrarás y podrás monitorear tus campañas.

En este artículo, abordamos la creación de campañas de retargeting; para ver una descripción completa de todas las funciones de esta página, consulta la [documentación de campañas](../product-documentation/demand-side-platform-dsp/).

### Creando una Campaña

1. En la [página principal de BMS](https://console.bluems.com/), haz clic en Campaigns, en la sección de campañas.
2. Haz clic en <img src="../.gitbook/assets/image (327).png" alt="" data-size="line"> para comenzar a crear tu campaña.
3. Asigna un Nombre y Etiquetas.
4. Selecciona tu dominio y zona horaria.
5. Define cuándo debe iniciar y finalizar la campaña.
6. Configura el precio de Puja (Bid):
   * Fija: esta opción usará el valor configurado para pujar. Ingresa aquí tu valor objetivo de CPM.
   * Variable: esta opción optimiza el costo de la puja dentro de un rango definido, buscando los valores más bajos posibles. Ingresa el valor mínimo y máximo de tu CPM.
7. Configura el límite de frecuencia (frequency cap), que define cuántas veces un anuncio de la misma campaña se mostrará al mismo usuario.
8. Define cuántas pujas deseas solicitar por segundo.
9. Haz clic en <img src="../.gitbook/assets/image (328).png" alt="" data-size="line"> para guardar tu campaña.

### Objetivo

Después de crear tu campaña, deberás configurar un objetivo para ella, en las campañas de retargeting, debes usar los pools de cookies como una de las opciones de objetivo, ya que el propósito es volver a atraer a los usuarios que interactuaron con tu sitio web, y el pool de cookies es la función que recopila estos datos, tienes otras opciones para ayudarte a construir tu objetivo ideal, incluyendo ubicación geográfica, idioma, categorías de dominios, dominios, palabras clave y Ad Exchanges.\
Nuestros objetivos funcionan con un sistema “Y” (AND), lo que significa que cada objetivo añadido a una campaña trabajará junto con los demás para ofrecerte una audiencia más específica y calificada.

#### Creación de un objetivo

1. Selecciona la campaña que recibirá este objetivo.
2. En la pestaña de Configuración, busca la sección Objetivo y haz clic en <img src="../.gitbook/assets/image (329).png" alt="" data-size="line"> para crear tu objetivo.
3. Establece un nombre para tu objetivo.
4. En la pestaña Ubicaciones, puedes definir la ubicación de tu objetivo:
   * Geografías: utilízalo para incluir o excluir países y regiones donde tu campaña debe ser entregada.
   * Geovallas: define una ubicación y un radio de distancia donde deseas que tu campaña se entregue.
5. En la pestaña Contenidos, encontrarás configuraciones importantes para tu objetivo:
   * Idiomas: selecciona el idioma de los sitios web donde se mostrarán tus anuncios; también puedes excluir idiomas que no desees.
   * Categorías: incluye categorías específicas para que tus anuncios solo aparezcan en sitios con contenido de esas categorías; también puedes excluir categorías para que tus anuncios no se muestren en sitios con contenido de esas categorías excluidas.
   * Dominios: incluye dominios específicos para que tus anuncios solo aparezcan en esos sitios; también puedes excluir dominios para que tus anuncios no se muestren en esos sitios excluidos.
   * Palabras clave de URL: incluye o excluye palabras clave de URL para refinar dónde aparecerán tus anuncios según el contenido de la URL.
6. En la pestaña Dispositivos, puedes definir parámetros para los dispositivos de tu objetivo:
   * Sistemas operativos: selecciona los sistemas operativos donde se mostrarán tus anuncios, o excluye los que no desees.
   * Navegadores: selecciona navegadores donde se mostrarán tus anuncios, o excluye los que no desees.
   * Tipos de dispositivos: selecciona tipos de dispositivos donde se mostrarán tus anuncios, o excluye los que no desees.
   * Palabras clave de URL visitadas: al definir palabras clave de URL visitadas, estás determinando qué dispositivos verán tus anuncios según su historial de navegación reciente. Rastreamos las URL a las que un dispositivo accedió en las últimas 24 horas.
   * Dominios visitados: al definir dominios visitados, estás determinando qué dispositivos verán tus anuncios según su historial de navegación reciente. Rastreamos los dominios a los que un dispositivo accedió en las últimas 24 horas.
   * Pools de cookies: selecciona pools de cookies para que tus anuncios apunten solo a los usuarios que han sido añadidos a esos pools seleccionados. También puedes excluir ciertos pools de cookies para que tus anuncios no apunten a los usuarios de esos pools excluidos. **Esta configuración es necesaria para las campañas de retargeting**.
7. En la pestaña Inventario, puedes configurar tus intercambios, visibilidad y posición de los anuncios:
   * Exchanges: selecciona los Ad Exchanges a través de los cuales se mostrarán tus anuncios, o excluye los que no desees.
   * Posición: selecciona las posiciones de inventario para colocar estratégicamente tus anuncios y optimizar su visibilidad e interacción; también puedes excluir posiciones.
   * Visibilidad: ajusta el control deslizante para definir el umbral mínimo de visibilidad para los espacios publicitarios. Tus anuncios solo se asociarán con posiciones donde el porcentaje de visibilidad sea superior al umbral seleccionado.
8. Haz clic en <img src="../.gitbook/assets/image (330).png" alt="" data-size="line"> para guardar tu objetivo.

### Presupuesto

Aquí configuras el presupuesto diario de tu campaña en USD. También puedes hacer un seguimiento de cuánto del presupuesto ya se ha gastado, cuánto aún tienes disponible y el objetivo actual de presupuesto.

1. En la pestaña Configuración, en la sección Presupuesto, informa el valor de tu presupuesto en USD.
2. Haz clic en <img src="../.gitbook/assets/image (330).png" alt="Save button" data-size="line"> para guardar tus cambios.

Ahora tu campaña de retargeting está lista para ejecutarse, solo debes habilitarla y seguir su rendimiento en las pestañas de métricas y tiempo real. Aquí tienes un artículo sobre [cómo funcionan las métricas en la plataforma BMS](../product-documentation/demand-side-platform-dsp/campaigns.md#metrics-tab).

{% hint style="info" %}
_Nuestra estrategia de puja funciona cruzando la información de la configuración de tu campaña y el conjunto de pujas definido, de modo que obtendrás impresiones basadas únicamente en la configuración de tu campaña_
{% endhint %}
