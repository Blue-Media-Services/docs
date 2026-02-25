# Canais de Importación

Utiliza los canales de importación para subir el feed del catálogo de tus productos a nuestra plataforma. Esta función también mantendrá tu catálogo actualizado según el feed.

## Gestión de Canales de Importación

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption><p>Lista de canales de importación</p></figcaption></figure>

### Creación de un Canal de Importación

Para empezar a crear un canal de importación, primero debemos crear el catálogo que contendrá los productos importados por el feed. Para crear un catálogo, siga los pasos que se indican en el [Catálogos](catalogs.md) artículo, también necesitaremos disponer de un feed de productos que utilicemos como fuente para nuestro canal de importación.

{% hint style="info" %}
_Los canales de importación pueden importar datos desde sitios web HTTP, FTP o SFTP. El formato XML de Google Merchant es el estándar para crear catálogos y el más fácil de manejar, pero el canal de importación se puede configurar para utilizar CSV u otros formatos XML._
{% endhint %}

1. Haga clic en <img src="../../.gitbook/assets/image (17) (2).png" alt="" data-size="line"> para empezar a crear tu canal de importación.
2.  Rellene los datos en las 3 pestañas:

    <figure><img src="../../.gitbook/assets/image (18) (1).png" alt=""><figcaption><p>Editor de Canales de Importación</p></figcaption></figure>

    1. Pestaña General\
       En esta pestaña encontrará los datos generales relacionados con su canal de importación. Utilice los ejemplos para ayudarle a rellenar todos los datos.
       * Nombre: Establezca un nombre para su canal de importación.
       * Etiquetas: Establezca etiquetas para su organización.
       * Catálogo: Seleccione el catálogo que ha creado para recibir los productos en el feed.
       * Cuándo crear o actualizar productos: Establezca el período en el que se crearán o actualizarán sus productos.
       * Cuándo eliminar productos:
         * Nunca: Los productos creados o actualizados en el origen se modificarán o añadirán al catálogo. Sin embargo, los productos eliminados en el origen no se eliminarán del catálogo.
         * Antes de cada importación: Todos los productos se eliminarán del catálogo antes de cada proceso de importación. A continuación, los productos que existan en el origen se añadirán al catálogo. ¡Atención! El catálogo permanecerá vacío hasta que se complete la importación, lo que podría dar lugar a banners publicitarios vacíos durante este periodo. Se conservarán todas las métricas de los productos.
         * Horas después de la importación: Defina cuánto tiempo deben permanecer los productos en el catálogo después de la importación si no se vuelven a importar. Siempre que la frecuencia de importación sea inferior al tiempo de caducidad del producto, el catálogo no quedará vacío. Se conservarán todas las métricas de los productos.&#x20;
    2.  Pestaña Fuente\
        Esta pestaña contiene los detalles de la fuente relacionados con su canal de importación. Utilice los ejemplos para ayudarle a rellenar estos detalles según su opción de fuente.

        * Protocolo: Seleccione el protocolo de su fuente y rellene los datos según su elección.
          1.  HTTP:

              <div align="center" data-full-width="false"><figure><img src="../../.gitbook/assets/Captura de tela 2024-08-27 121710.png" alt=""><figcaption><p>Pestaña Fuente - HTTP</p></figcaption></figure></div>

              * URL: Indique la URL de su feed.
          2.  SFTP y FTP:

              <figure><img src="../../.gitbook/assets/Captura de tela 2024-08-22 090041.png" alt=""><figcaption><p>Pestaña Fuente - SFTP/FTP</p></figcaption></figure>

              * Host: Indique el host de su fuente.
              * Puerto: Indique el puerto de su fuente.
              * Usuario: Indique un usuario para acceder a su fuente.
              * Contraseña: Indique la contraseña para validar su usuario en la fuente.
              * Ruta: Indique la ruta a su fuente.
        * Fuente de prueba: Este botón, <img src="../../.gitbook/assets/image (905).png" alt="" data-size="line">, le permite probar su fuente y recuperar datos relevantes para los siguientes campos. Hay tres pestañas para el resultado de la prueba de la fuente:
          * Registros detectados: muestra los registros de tu feed en formato de tabla.
          * Problemas: muestra los problemas que pueden afectar a tu trabajo de importación.
          *   Sin procesar: muestra el código fuente de tu archivo de feed.

              <figure><img src="../../.gitbook/assets/image (904).png" alt=""><figcaption><p>Resultado de la prueba de origen</p></figcaption></figure>

        Después de terminar la prueba, haga clic en <img src="../../.gitbook/assets/image (992).png" alt="" data-size="line"> para cerrar la ventana de resultados de la prueba de origen y rellenar automáticamente los siguientes campos con los resultados de la prueba.

        * Juego de caracteres: Indique el juego de caracteres de la fuente, que se detectó previamente en el resultado de la prueba de la fuente.
        * Formato de archivo: El resultado de la prueba de la fuente rellenará automáticamente estos campos, sin embargo, puede cambiarlos manualmente. Seleccione entre estas opciones:
          * CSV: Fuente basada en un archivo con valores separados por comas.
            * Delimitador: inserte el carácter que separa los valores de su archivo.
          * XML: Fuente basada en un archivo XML.
            * Etiqueta de elemento: inserte la etiqueta de elemento en su archivo XML.
    3.  Pestaña Mapeo\
        En esta pestaña encontrará los detalles de asignación relacionados con su canal de importación. Utilice los ejemplos para ayudarle a configurar su asignación.

        *   Formato de plantilla: Seleccione entre estas dos opciones:

            * Google Shopping: Seleccione esta opción si utiliza un feed de Google Shopping.

            <figure><img src="../../.gitbook/assets/image (987).png" alt=""><figcaption><p>Pestaña Mapeo - Google Shopping</p></figcaption></figure>

            * Avanzado: Para cualquier otro tipo de archivo de fuente, seleccione esta opción.

            <figure><img src="../../.gitbook/assets/image (903).png" alt=""><figcaption><p>Pestaña Mapeo - Avanzado</p></figcaption></figure>
        * Detectar plantilla: Haga clic en <img src="../../.gitbook/assets/image (994).png" alt="" data-size="line"> detectar la mejor plantilla basada en tu archivo de alimentación.
        * Plantilla de prueba: Haga clic en <img src="../../.gitbook/assets/image (911).png" alt="" data-size="line"> para acceder a una vista previa de cómo se mostrarán sus productos en su catálogo. Si hay algún error en la asignación o en el archivo de alimentación, lo notará en esta prueba.

        <figure><img src="../../.gitbook/assets/Captura de tela 2024-09-18 145710.png" alt=""><figcaption><p>Resultado de la prueba de mapeo</p></figcaption></figure>

        * Haga clic en <img src="../../.gitbook/assets/image (999).png" alt="" data-size="line"> para continuar.
    4.  Pestaña Filtros\
        En esta pestaña, podrás establecer filtros para seleccionar los productos que necesitas importar. Esto puede ser útil para reducir los costes de los trabajos de importación, ya que solo se importarán los productos que necesites.

        * Ruta: Indique un valor de ruta, como una de las etiquetas de columna de la fuente.
        * Operador: Seleccione uno de los valores del operador, este valor establecerá el filtro.
        * Valor: Indique el valor que necesita filtrar del feed de su catálogo, como el nombre de una marca o un rango de identificadores de productos.
        * Después de rellenar los campos, también deberá introducir los mismos datos en la plantilla que se muestra. Solo debe cambiar los valores que está filtrando, de lo contrario, no funcionará correctamente.

        Puede añadir tantos filtros como sea necesario haciendo clic en <img src="../../.gitbook/assets/image (441) (1).png" alt="" data-size="original">, y también eliminarlos haciendo clic en ![](<../../.gitbook/assets/image (998).png>) en la misma fila que el filtro que desea eliminar.

        <figure><img src="../../.gitbook/assets/Captura de tela 2024-12-19 110001.png" alt=""><figcaption><p>Pestaña Filtros</p></figcaption></figure>

        * _**Ejemplo 1:** En esta imagen, notará que se estableció un filtro utilizando la columna de descripción del archivo del feed como referencia para la ruta; el operador elegido fue "Contains" (Contiene) y el Valor fue "Cerdo", lo que significa que este canal de importación solo importará productos que contengan la palabra "Cerdo" en su descripción. También notará que en la plantilla, el contenido de la línea "description" se modificó para coincidir con el valor del filtro._
        * _**Ejemplo 2:** También notará un filtro que utiliza la columna "url" como referencia para la ruta; este fue añadido manualmente. Para añadir manualmente nuevas columnas a sus filtros, estas deben estar presentes también en el mapeo de su feed. Asimismo, debe respetar la semántica de la plantilla: las columnas se separan por comas y se utilizan los dos puntos para separar la etiqueta de una columna de su valor. Las etiquetas de las columnas y los valores deben declararse entre comillas._
3. Una vez que haya completado los pasos anteriores, compruebe la configuración para asegurarse de que todo sea correcto y, a continuación, haga clic en <img src="../../.gitbook/assets/image (19) (1).png" alt="" data-size="line"> para guardar tu canal de importación.
4.  Haga clic en <img src="../../.gitbook/assets/image (10).png" alt="" data-size="original"> para iniciar una tarea manual para importar sus productos:

    <figure><img src="../../.gitbook/assets/image (11) (1).png" alt=""><figcaption><p>Iniciar pantalla de trabajos</p></figcaption></figure>
5. Haga clic en <img src="../../.gitbook/assets/image (12).png" alt="" data-size="line"> para comenzar a importar sus productos.
6.  También es posible importar solo algunos productos para comprobar si todo funciona correctamente antes de iniciar la importación completa. Para ello, marque la casilla "Modo de prueba", rellene los datos y haga clic en <img src="../../.gitbook/assets/image (12) (1).png" alt="" data-size="line">.

    <figure><img src="../../.gitbook/assets/image (398).png" alt=""><figcaption><p>Pantalla Iniciar trabajos - Modo de prueba</p></figcaption></figure>
7.  Sigue tu importación en la pestaña Trabajos. En esta pestaña podemos ver los problemas con nuestra importación o si se han completado. Es posible comprender el problema haciendo clic en ![](<../../.gitbook/assets/image (59) (1).png>) o ![](<../../.gitbook/assets/image (262).png>) en la misma fila que el trabajo fallido.

    <figure><img src="../../.gitbook/assets/image (259).png" alt=""><figcaption><p>Pestaña de Trabajos</p></figcaption></figure>

### Edición de un Canal de Importación

Podemos editar nuestros canales de importación haciendo clic en <img src="../../.gitbook/assets/image (13).png" alt="" data-size="line"> en la misma fila que el canal de importación que necesita editar. Todos los detalles están disponibles para su edición.

### Eliminación de un Canal de Importación

Podemos eliminar los canales de importación que no se utilizan haciendo clic en <img src="../../.gitbook/assets/image (15).png" alt="" data-size="line"> en la misma fila en la que se encuentra el canal de importación que se va a eliminar; sin embargo, esto también eliminará las métricas relacionadas con él, por lo que se debe proceder con precaución. Como alternativa, también podemos archivar estos canales de importación haciendo clic en <img src="../../.gitbook/assets/image (14).png" alt="" data-size="line"> en la misma fila que el canal de importación que se va a archivar, para ver los canales de importación archivados, active la opción "Archivado" situada encima de la lista de canales de importación.

## Pestaña Métricas

La pestaña de métricas de canales de importación contiene datos sobre sus trabajos de importación, como el procesamiento de datos, el rendimiento y la tasa de fallos. La pestaña de métricas mostrará los datos de toda la cuenta para todos los canales de importación si no se selecciona ningún canal de importación. Al seleccionar un solo canal de importación, se mostrarán las métricas específicas de ese canal, mientras que al seleccionar varios canales de importación se comparará su rendimiento. Estas son las métricas disponibles para los canales de importación:&#x20;

* [Recuento de trabajos de Importación](cs2-metrics.md#import-job-count)
* [Duración de trabajos de Importación](cs2-metrics.md#import-job-duration)
* [Tasa de fallos de trabajos de Importación](cs2-metrics.md#import-job-failure-rate)
* [Problemas de trabajos de Importación](cs2-metrics.md#import-job-issues)
* [Bytes procesados ​​de trabajos de Importación](cs2-metrics.md#import-job-processed-bytes)
* [Registros procesados ​​de trabajos de Importación](cs2-metrics.md#import-job-processed-records)
