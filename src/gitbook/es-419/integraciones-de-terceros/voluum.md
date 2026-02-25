# Voluum

Voluum es una plataforma de análisis basada en la nube que ayuda a los profesionales del marketing a supervisar, optimizar y analizar sus campañas digitales. Gestiona grandes volúmenes de datos y proporciona información en tiempo real sobre métricas clave como clics, conversiones y ROI.

## Seguimiento de Campañas BMS con Voluum

Al integrar BMS con Voluum, los anunciantes pueden exportar datos de campañas, realizar un seguimiento de eventos específicos y obtener una visibilidad más profunda del rendimiento de sus campañas.

<figure><img src="../.gitbook/assets/image (504).png" alt=""><figcaption><p>Página de inicio de Voluum</p></figcaption></figure>

### Seguimiento de Clics e Impresiones

{% hint style="info" %}
Este artículo se centra en la integración de **BMS** como fuente de tráfico en **Voluum**. No trataremos todas las opciones de creación de campañas de Voluum. Para obtener más información sobre las funciones de Voluum, visite nuestro [**Información Adicional**](voluum.md#additional-information) sección o [Documentación de Voluum](https://doc.voluum.com/).
{% endhint %}

Debes añadir BMS como fuente de tráfico en tus campañas de Voluum para extraer datos.

1. Selecciona la pestaña "Campañas".
2. Haga clic en "Crear" para crear una nueva campaña.
3.  Selecciona "Simple" como modo de creación.

    <figure><img src="../.gitbook/assets/image (505).png" alt=""><figcaption><p>Editor de campañas de Voluum - Pestaña General</p></figcaption></figure>
4. Rellene los datos:
   * **General**
     * **Fuente de tráfico:** Busque "BMS" y selecciónelo.
     * **Tipo de Tráfico:** Seleccione el tipo de tráfico en función del tipo de su campaña, por ejemplo, Banner.
     * **Etiqueta de País:** Seleccione el país en el que se está ejecutando su campaña.
     * **Modelo de Coste:** Seleccione el modelo de coste aplicado a su campaña.
5. Cuando esté satisfecho con los parámetros restantes, haga clic en Guardar para continuar.
6.  Seleccione la pestaña Seguimiento y automatización.

    <figure><img src="../.gitbook/assets/image (4) (1).png" alt=""><figcaption><p>Editor de campañas de Voluum: pestaña Seguimiento y automatización</p></figcaption></figure>
7.  Aquí encontrará dos datos fundamentales que concluirán el proceso de integración:

    *   **URL de la Campaña:** Este parámetro permitirá a Voluum realizar un seguimiento de los clics en sus campañas de BMS. Utilice el botón Copiar para copiar este enlace y, a continuación, utilícelo como enlace de su anuncio, es decir, péguelo en el parámetro "Enlace a" de sus anuncios o creatividades.

        <figure><img src="../.gitbook/assets/image (1043).png" alt=""><figcaption><p>Editor creativo - Enlace a</p></figcaption></figure>
    * **URL de clic de Impresión:** Este parámetro permitirá a Voluum realizar un seguimiento de las impresiones en sus campañas BMS. Debe copiarlo utilizando el botón Copiar, pegar esta URL dentro de una etiqueta de píxel como fuente y, a continuación, añadir esta etiqueta de píxel a su código HTML creativo.
      * _**Ejemplo:**_ Este es un ejemplo de una etiqueta de píxel:\
        `<img src="VOLUUM_IMPRESSION_PIXEL_URL" style="position: absolute; opacity: 0;">`\
        Debes sustituir el parámetro 'src' por el enlace que has copiado de Voluum. Tras sustituirlo, obtendrás un resultado como este:\
        `<img src="https://ImpressionURL.copied/from/Voluum" style="position: absolute; opacity: 0;">`

    <figure><img src="../.gitbook/assets/image (795).png" alt=""><figcaption><p>Editor creativo - Pestaña Pegar HTML</p></figcaption></figure>

## Información Adicional

Después de seguir los pasos anteriores, comenzará a recibir los datos de sus campañas BMS en Voluum y la integración habrá finalizado. También puede consultar los siguientes artículos para obtener más información sobre nuestro proceso de creación de anuncios y otras funciones de Voluum.

* [Creativos](../product-documentation/ad-server/creatives.md)
* [Anuncios](../product-documentation/ad-server/ads/)
* [Crear una campaña de Voluum](https://doc.voluum.com/article/create-a-voluum-campaign)
* [Agregar una Fuente de Tráfico a Voluum](https://doc.voluum.com/article/add-a-traffic-source-to-voluum)
* [Añade una red de Afiliados a Voluum](https://doc.voluum.com/article/add-an-affiliate-network-to-voluum)
