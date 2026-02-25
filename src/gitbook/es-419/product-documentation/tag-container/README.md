# Contenedores de Etiquetas

Esta función le permite crear un contenedor de etiquetas personalizado para instalar varias etiquetas y scripts desde un único fragmento de código.

<figure><img src="../../.gitbook/assets/image (537).png" alt=""><figcaption><p>Lista de contenedores de Etiquetas</p></figcaption></figure>

### Creación de Contenedores de Etiquetas

Siga los pasos que se indican a continuación para crear su contenedor de etiquetas. Este proceso le guiará a través de los pasos necesarios para configurar un contenedor personalizado que pueda albergar múltiples etiquetas y scripts, lo que simplificará la gestión y la implementación de códigos de seguimiento en su sitio web.

{% hint style="info" %}
Utilizamos grupos de cookies y rastreadores como ejemplos de scripts para explicar esta función, pero puede utilizar cualquier script o etiqueta que necesite.
{% endhint %}

1.  Haga clic en <img src="../../.gitbook/assets/image (522).png" alt="" data-size="line"> para empezar a crear tu contenedor de etiquetas.

    <figure><img src="../../.gitbook/assets/image (521).png" alt=""><figcaption><p>Editor de contenedores de etiquetas</p></figcaption></figure>
2. Rellene los datos:
   * Nombre: Establezca un nombre para su contenedor de etiquetas.
   * Etiquetas: Establece etiquetas para organizar mejor tus archivos.
   * Plantilla: Pega los scripts y las etiquetas que necesites incluir en tu contenedor de etiquetas. En el ejemplo mostrado, se utilizó un script de Cookie Pool de BMS. Observa que los valores del ID de cuenta ("acc") y del ID de Cookie Pool ("cpid") fueron sustituidos por los marcadores de posición "\{{acc\}}" y "\{{cpid\}}". Esto permite que el contenedor de etiquetas se utilice de forma dinámica. Del mismo modo, también se añadió un script de seguimiento (tracker) de BMS.
   * Parámetros disponibles: Los parámetros aparecerán en esta sección según su entrada de muestra. Puede hacer clic en ellos para copiar sus referencias.
   * Entrada de muestra: Aquí es donde proporcionará una entrada de muestra para su contenedor de etiquetas. En el ejemplo que se muestra, hay cuatro parámetros configurados en la entrada de muestra:
     * "e": Se refiere al evento que debe rastrearse utilizando nuestro script de rastreo.
     * "t": Se refiere al ID del rastreador que se va a utilizar.
     * "acc": Se refiere al ID de la cuenta BMS.
     * "cpid": Se refiere al ID del Cookie Pool.
   * Vista previa: Esta sección muestra cómo quedará tu contenedor de etiquetas después de rellenar los parámetros.
3. Después de terminar tus ediciones, haz clic en <img src="../../.gitbook/assets/image (524).png" alt="" data-size="line"> para guardar tu contenedor de etiquetas.

### Instalación de su Contenedor de Etiquetas

Siga los pasos que se indican en la pestaña de instrucciones de instalación para instalar correctamente su contenedor de etiquetas.

<figure><img src="../../.gitbook/assets/image (525).png" alt=""><figcaption><p>Pestaña Instrucciones de instalación</p></figcaption></figure>

1. Copie el script utilizando el botón copiar <img src="../../.gitbook/assets/image (526).png" alt="" data-size="line">.
2. Reemplace los parámetros con los valores correspondientes.
3. Pégalo en el código de tu sitio web.

### Edición o eliminación de Contenedores de Etiquetas

Todos los campos del editor del contenedor de etiquetas están disponibles para su edición, haga clic en <img src="../../.gitbook/assets/image (527).png" alt="" data-size="line"> para editar tu contenedor de etiquetas.

{% hint style="danger" %}
¡Atención! Tenga cuidado al eliminar contenedores de etiquetas, ya que esta acción no se puede deshacer y todos los datos relacionados, incluidas las métricas recopiladas anteriormente, también se eliminarán.
{% endhint %}

Es posible eliminar contenedores de etiquetas haciendo clic en <img src="../../.gitbook/assets/image (528) (1).png" alt="" data-size="line"> en la misma fila que el contenedor de etiquetas que desea eliminar y, a continuación, haciendo clic en <img src="../../.gitbook/assets/image (529).png" alt="" data-size="line"> para confirmar esta acción.

Como alternativa, puede archivar contenedores de etiquetas para facilitar la organización. Para ello, haga clic en <img src="../../.gitbook/assets/image (530) (1).png" alt="" data-size="line"> en la misma fila que el contenedor de etiquetas que desea archivar. Para ver los contenedores de etiquetas archivados, active el interruptor "Archivado" ![](<../../.gitbook/assets/image (531).png>), situado justo encima de la lista de contenedores de etiquetas. Para desarchivar un contenedor de etiquetas, haga clic en <img src="../../.gitbook/assets/image (532).png" alt="" data-size="line"> en la misma fila que el contenedor de etiquetas que desea desarchivar.

### Pestaña Métricas

Una vez finalizada la instalación de los contenedores de etiquetas y tras utilizarlos de forma eficaz, estos comenzarán a cumplir con las métricas presentadas. A continuación, encontrará todas las métricas relacionadas con los contenedores de etiquetas:

* [Tasa de Fallos](metricas-de-contenedores-de-etiquetas.md#failure-rate)
* [Número de Solicitudes](metricas-de-contenedores-de-etiquetas.md#request-count)
