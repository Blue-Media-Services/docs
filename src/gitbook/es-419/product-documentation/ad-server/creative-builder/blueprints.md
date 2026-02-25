---
description: ¡Más información sobre los planos y cómo trabajar con ellos!
---

# Blueprints

Los planos son modelos para crear anuncios de forma rápida y eficaz. Estos modelos predefinidos te permiten programar banners dinámicos utilizando lenguajes de desarrollo web, lo que te permite crear anuncios más atractivos y mejorar los resultados esperados.

Basados en lenguajes de diseño web, los Blueprints ofrecen la flexibilidad de crear banners dinámicos. Aunque no estés familiarizado con los lenguajes de desarrollo web, puedes utilizar con confianza uno de los Blueprints predefinidos disponibles.

## Gestión de Blueprints

<figure><img src="../../../.gitbook/assets/Captura de tela 2024-12-05 072802.png" alt=""><figcaption><p>Lista de Blueprints</p></figcaption></figure>

Tendrás a tu disposición algunos modelos de planos públicos, por lo que, aunque no estés familiarizado con los lenguajes de desarrollo web, podrás crear y utilizar planos fácilmente. También puedes crear un plano con tus parámetros mediante la codificación; sin embargo, esta opción puede requerir conocimientos de desarrollo web.

### Creación de Blueprint

Haga clic en ![create blueprint](<../../../.gitbook/assets/image (803).png>) para empezar a crear tu plan.

<figure><img src="../../../.gitbook/assets/image (800).png" alt=""><figcaption><p>Creación de Blueprint</p></figcaption></figure>

1. Rellene los datos:
   * Nombre: Establezca un nombre para su plano.
   * Etiquetas: Establece etiquetas para organizar mejor tus archivos.
   * Disponibilidad: Seleccione si desea que este plano sea público o privado. Los planos públicos estarán disponibles para todos los usuarios de BMS.
   * Generar tamaños: seleccione en qué tamaños se crearán sus creatividades a partir de este modelo.
   *   Parámetros: Haga clic en ![](<../../../.gitbook/assets/image (69) (2).png>) para crear un nuevo grupo de parámetros.

       <figure><img src="../../../.gitbook/assets/image (327).png" alt=""><figcaption><p>Creador de grupos de parámetros</p></figcaption></figure>

       * Nombre: Establezca un nombre para este grupo de parámetros.
       * Descripción: Establezca una descripción del grupo de parámetros.
       * Haga clic en ![save](<../../../.gitbook/assets/image (806).png>) para guardar su grupo de parámetros.
2.  Después de crear el grupo de parámetros, puede comenzar a codificar su banner en el cuadro de código. A continuación, configure los parámetros de su código para que coincidan con los del grupo de parámetros. Para añadir un nuevo parámetro al grupo, haga clic en ![](<../../../.gitbook/assets/image (224).png>) y rellene los datos:

    <figure><img src="../../../.gitbook/assets/image (249).png" alt=""><figcaption><p>Creador de parámetros - Opciones de tipo</p></figcaption></figure>

    * ID del parámetro: utilice este identificador para insertar el valor de usuario proporcionado en su plantilla.
    * Nombre: Asigne un nombre a su parámetro.
    * Descripción: Establezca una descripción para su parámetro.
    * Tipo: Seleccione el tipo de datos de la entrada:
      *   **String**

          <figure><img src="../../../.gitbook/assets/image (328).png" alt=""><figcaption><p>Editor de parámetros - Tipo String</p></figcaption></figure>

          * Longitud mínima: Establece una longitud mínima para la entrada.
          * Longitud máxima: Establece una longitud máxima para la entrada.
          * Expresión regular de validación: Introduzca el patrón utilizado para la validación de la String.
          * Mensaje de validación: este mensaje se muestra al usuario si el patrón de validación no coincide.
          * Seleccione entre las siguientes opciones:
            * Una sola línea: Crea un campo para introducir una sola línea de texto.
            * Multilínea: Crea un campo que permite introducir varias líneas de texto.
          * Valor inicial: Es el valor inicial que utilizará el sistema al crear una nueva compilación.
      *   **Booleano**

          <figure><img src="../../../.gitbook/assets/image (247).png" alt=""><figcaption><p>Editor de parámetros - Tipo Booleano</p></figcaption></figure>

          * Valor inicial: Marque la casilla si el valor inicial es verdadero, desmárquela si es falso.
      *   **Elección**

          <figure><img src="../../../.gitbook/assets/image (248).png" alt=""><figcaption><p>Editor de parámetros - Tipo Elección</p></figcaption></figure>

          * Etiqueta: Introduzca la etiqueta de su parámetro.
          * Valor: Introduzca el valor asociado a la etiqueta.
          * Añade tantas etiquetas como necesites haciendo clic en ![Add](<../../../.gitbook/assets/image (805).png>).
          * Valor inicial: Seleccione una de las etiquetas configuradas como valor inicial.
      *   **Código**

          <figure><img src="../../../.gitbook/assets/image (250).png" alt=""><figcaption><p>Editor de parámetros - Tipo Código</p></figcaption></figure>

          * Tipo: Seleccione el lenguaje del código.
          * Cuadro de código: Introduzca su código en el cuadro de código.
      *   **Color**

          <figure><img src="../../../.gitbook/assets/image (244).png" alt=""><figcaption><p>Editor de parámetros - Tipo Color</p></figcaption></figure>

          * Valor inicial: Introduzca el código hexadecimal del color o haga clic en el cuadro de color para seleccionar un color.
      *   **Número**

          <figure><img src="../../../.gitbook/assets/image (246).png" alt=""><figcaption><p>Editor de parámetros - Tipo Número</p></figcaption></figure>

          * Mínimo: Introduzca el valor mínimo que se aceptará.
          * Máximo: Introduzca el valor máximo que se aceptará.
          * Valor inicial: Introduzca el valor inicial del parámetro.
      *   **ID de recurso**

          <figure><img src="../../../.gitbook/assets/image (245).png" alt=""><figcaption><p>Editor de parámetros - Tipo de ID de recurso</p></figcaption></figure>

          * Tipo de recurso: elija entre un catálogo CS2 o un modelo de recomendación CS2 para utilizar uno de ellos como recurso para su banner.
          * Valor inicial: seleccione el catálogo específico o el modelo de recomendación que desea utilizar para este parámetro.
      *   **URL**

          <figure><img src="../../../.gitbook/assets/image (329).png" alt=""><figcaption><p>Editor de parámetros - Tipo URL</p></figcaption></figure>

          * Usar selector de imágenes: marque esta casilla para habilitar el selector de imágenes, en el que puede seleccionar imágenes de sus creatividades cargadas, cargar una nueva si es necesario o informar la URL de la imagen.
          * Valor inicial: inserte el valor inicial para la URL de la imagen.
    * Haga clic en ![save](<../../../.gitbook/assets/image (806).png>) para guardar tu parámetro.
3. Continúe añadiendo grupos de parámetros y parámetros hasta satisfacer las necesidades de su negocio.
4. Utiliza los parámetros del sistema disponibles para personalizar tu plantilla:
   * ID de cuenta: esta opción inserta en tu plantilla el ID de la cuenta en la que se crea la compilación.
   * Ancho del banner: inserta el ancho con el que se mostrará el banner.
   * Altura del banner: inserta la altura con la que se mostrará el banner.
5. Utiliza las **macros** disponibles con tus URL, algunas de ellas son:
   * **URL de clic sin escapar:** esta macro se sustituirá por la URL del rastreador de clics sin escapar de BMS. Utilice esta opción cuando BMS sea el primer rastreador de clics de la cadena.
   * **URL de clic escapado:** esta macro se sustituirá por la URL del rastreador de clics escapado de BMS. Utilice esta opción cuando BMS sea el segundo rastreador de clics de la cadena.&#x20;
   * **URL de clic doblemente escapado:** Esta macro se sustituirá por la URL del rastreador de clics doblemente escapada de BMS. Utilice esta opción cuando BMS sea el tercer rastreador de clics de la cadena.
   * **Cache Buster:** Esta macro se sustituirá por un número aleatorio que se puede utilizar para eliminar la caché.
   * **Contexto publicitario escapado:** Esta macro se sustituirá por un objeto JSON escapado que contiene datos sobre el contexto publicitario, como el ID de la campaña y los datos de los usuarios.&#x20;
6. Después de terminar todos los ajustes del plano, haga clic en <img src="../../../.gitbook/assets/image (9) (1).png" alt="" data-size="line"> para guardar tu plano.

### Usar un plano existente

También es posible utilizar un plano existente. Puede duplicar un plano que ya tenga para reutilizar algunos de sus parámetros haciendo clic en <img src="../../../.gitbook/assets/image (227).png" alt="" data-size="line"> en la misma fila que el plano que desea duplicar. Además, puede utilizar un plano público. Desactive la opción <img src="../../../.gitbook/assets/image (228).png" alt="" data-size="line"> opción propia, encima de la lista de planos, elige uno de los planos disponibles y haz clic en <img src="../../../.gitbook/assets/image (227).png" alt="" data-size="line"> en la misma fila que el plano público que desea utilizar. Active ![](<../../../.gitbook/assets/image (230).png>)la opción de propiedad de nuevo y, a continuación, haga clic en <img src="../../../.gitbook/assets/image (232).png" alt="" data-size="line"> para editar el plano según las necesidades de su negocio.

### Eliminación de planos

Puede eliminar o archivar planos según sus necesidades. Para archivar planos, haga clic en ![](<../../../.gitbook/assets/image (233).png>) en la misma fila que el plano que desea archivar. Para ver sus planos archivados, active la opción ![](<../../../.gitbook/assets/image (230).png>) opción archivada encima de la lista de planos.

{% hint style="danger" %}
Ten cuidado al eliminar planos, ya que esta acción no se puede deshacer y las compilaciones que dependen del plano eliminado dejarán de funcionar. Además, todos los datos relacionados, incluidas las métricas recopiladas anteriormente, también se eliminarán.
{% endhint %}

Para eliminar planos, haga clic en ![](<../../../.gitbook/assets/image (321).png>) en la misma fila que el plano que desea eliminar, luego confirme la acción haciendo clic en <img src="../../../.gitbook/assets/image (236).png" alt="" data-size="line">.
