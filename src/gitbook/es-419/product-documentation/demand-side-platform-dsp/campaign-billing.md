# Facturación de Campañas

La sección de Facturación de Campañas contendrá todos los elementos facturados relacionados con las campañas y se divide en dos subsecciones.

<figure><img src="../../.gitbook/assets/image (566).png" alt=""><figcaption><p>Sección de Facturación de Campañas</p></figcaption></figure>

{% hint style="info" %}
En BMS, se prioriza la transparencia mostrando todos los detalles de su factura. Visite nuestra [Facturación](../billing.md) para comprender cómo están estructurados los proyectos de ley.
{% endhint %}

## ¿Cómo se compone su facturación?

Al crear e iniciar una campaña, es necesario utilizar varios productos y funciones de nuestra plataforma para tener todo listo para comenzar la campaña. Tenga en cuenta que la facturación de la campaña no solo se basa en el presupuesto diario establecido.

### Facturación X Presupuesto

Nuestra facturación se basa en el uso de cada producto, es decir, el coste efectivo de cada producto según su uso, medido por cada solicitud enviada a una **API**, **almacenamiento** y **medios**.

### Almacenamiento

Al ejecutar una campaña, se utilizan varios productos para crear sus componentes. Como resultado, el almacenamiento de cada elemento creativo, grupo creativo, anuncio y elemento multimedia generará gastos. En los casos en que la cuenta acumule demasiados elementos de este tipo, podría producirse un impacto significativo en la facturación mensual. Por lo tanto, realizar limpiezas periódicas de los elementos no utilizados es una buena práctica para mantener un saldo de facturación manejable.&#x20;

**Ejemplo:** Incluso cuando una campaña está inactiva, es posible que se sigan aplicando cargos, ya que los creativos y los anuncios creados para esa campaña siguen generando costes de almacenamiento.

### Medios

Todos los archivos multimedia cargados en la biblioteca generan costes de almacenamiento y descarga. Cada vez que un usuario final ve tus archivos multimedia en una campaña, se genera un coste tanto por el almacenamiento como por la descarga. Estos costes varían en función del tamaño de cada archivo multimedia, ya que consumen espacio de almacenamiento en los servidores de BMS. Para ayudar a gestionar estos gastos, considera la posibilidad de utilizar archivos multimedia alojados en tus propios servidores.&#x20;

**Ejemplo:** Un archivo multimedia con un tamaño de 3 MB tendrá un coste diferente al de uno con un tamaño de 5 MB. Al alojar ese archivo multimedia en su propio servidor, BMS no le cobrará por él.

### Presupuesto Diario

El presupuesto diario establecido para una campaña funciona como un acelerador, ayudándote a controlar cuánto pretendes gastar. La cantidad real gastada al final del día puede variar en función de las configuraciones de los objetivos, los ajustes de puja y los medios utilizados en la campaña.

Una vez establecido el presupuesto diario, este se utiliza en cuatro tipos diferentes para llevar a cabo una campaña de forma completa: **impresiones**, **entregas**, **pujas** y **recomendaciones**.

#### Presupuesto gastado en Impresiones

Este presupuesto se gasta en función de las pujas ganadas, y el importe se paga al editor por el derecho a mostrar anuncios en su sitio web. En la facturación, esto se representa como el coste de los medios (la suma de todas las pujas ganadoras) más una comisión del 20 % por la plataforma.

<figure><img src="../../.gitbook/assets/image (920).png" alt=""><figcaption><p>Presupuesto gastado en la métrica de Impresiones</p></figcaption></figure>

**Ejemplo:** En este caso, el presupuesto gastado en impresiones fue de más de 0,50 $ hasta un máximo de 0,75 $; esta métrica se mostrará en la gestión del presupuesto y los medios como el coste de los medios; al eliminar la tarifa de la plataforma del 20 %, es posible hacer coincidir los valores.

<figure><img src="../../.gitbook/assets/image (835).png" alt=""><figcaption><p>Presupuesto gastado en facturación por Impresiones</p></figcaption></figure>

#### Presupuesto gastado en Entregas

Este presupuesto se refiere al coste total de entrega de un anuncio, que incluye los gastos combinados del Ad Server, la supervisión y los medios. El coste del Ad Server cubre las solicitudes de API necesarias para entregar el anuncio, los costes de supervisión capturan las métricas y las muestran en el panel de control, y los costes de los medios cubren la descarga de los medios asociados. En la facturación, estos costes aparecen en las partidas **Ad Server**, **Medios** y **Supervisión**. Este coste puede variar en función del tamaño de los medios; los archivos multimedia más grandes supondrán gastos más elevados.&#x20;

<figure><img src="../../.gitbook/assets/image (836).png" alt=""><figcaption><p>Presupuesto gastado en Entregas Métrica</p></figcaption></figure>

**Ejemplo:** En esta métrica se puede ver que cada hora se gastan entre 0,01 $ y 0,025 $ solo en entregas. Este valor se deducirá del presupuesto diario, aunque no esté relacionado con la puja en sí.

#### Presupuesto gastado en Pujas

Este coste está asociado al gasto operativo de realizar pujas. Cada vez que se realiza una puja, esta se ajusta a los objetivos de la campaña, lo que requiere que el sistema filtre todo el inventario disponible en función de las preferencias de la campaña para garantizar una puja precisa. Este proceso conlleva gastos, aunque representan un pequeño porcentaje del presupuesto diario total. En su extracto de facturación, la sección "Pujas en tiempo real" incluirá una partida denominada "Pujas realizadas", que se corresponde con las métricas de pujas de su campaña.&#x20;

<figure><img src="../../.gitbook/assets/image (919).png" alt=""><figcaption><p>Presupuesto gastado en Pujas Métrica</p></figcaption></figure>

**Ejemplo:** En esta métrica, se observa que el presupuesto gastado en costes operativos ha sido superior a 0,05 $ hasta un máximo de 0,13 $; este coste aparecerá en su factura como "Real Time Bidding" (puja en tiempo real) y coincidirá con los costes operativos de su campaña.

<figure><img src="../../.gitbook/assets/image (918).png" alt=""><figcaption><p>Realización de Pujas Facturación</p></figcaption></figure>

#### Presupuesto gastado en Recomendaciones

Al utilizar banners dinámicos, se le cobrará por utilizar la llamada a la API para una recomendación, debido al coste operativo que supone vincular sus objetivos a una recomendación. Si una campaña no utiliza banners dinámicos, no habrá ningún coste.

<figure><img src="../../.gitbook/assets/image (794).png" alt=""><figcaption><p>Presupuesto gastado con Recomendaciones Métricas</p></figcaption></figure>

**Ejemplo:** En esta métrica, se observa que el presupuesto gastado fue de más de 0,05 $ hasta 0,08 $ cada 12 horas, valor que se deduce del presupuesto diario de la campaña.

## Gestión Presupuestaria y Medios de Comunicación

En la gestión presupuestaria y los medios, las facturas relacionadas con BMS muestran la disponibilidad presupuestaria actual, las solicitudes generadas al cambiar o establecer un presupuesto para una campaña y el coste de los medios más un impuesto BMS del 20 %. El coste de los medios se basa en la cantidad pagada a un editor por mostrar su anuncio.

<figure><img src="../../.gitbook/assets/image (567).png" alt=""><figcaption><p>Gestión Presupuestaria y Elementos Multimedia</p></figcaption></figure>

**Ejemplo:** En esta factura, se indica un coste de medios de 4.014,89 $ más CPM. Este coste se basa en 3.345,74 $, que se transferirán a los editores que mostraron su anuncio, y 669,15 $ adicionales del impuesto del 20 % por utilizar el postor de BMS. También se cobró la disponibilidad del presupuesto de la campaña por superar las 1 000 000 de solicitudes. A un coste de 0,10 $ por cada 1 000 000 de solicitudes, el total ascendió a 0,72 $. Tras sumar todas las facturas, el coste total alcanzó los 4015,61 $.&#x20;

## Gestión de Campañas

En la factura de gestión de campañas, se mostrarán los costes de cualquier acción realizada en la página de la campaña y del almacenamiento de la misma. Cada vez que crees, actives o desactives campañas, se contará como una solicitud. Si el número de solicitudes supera las 1000 durante un mes, se aplicará un coste. Las campañas se cobran incluso si están inactivas. BMS cuenta cada segundo que una campaña está listada, ya sea activa o no, y convierte los segundos en horas, cobrando 0,75 dólares por campaña al mes, basándose en un mes de 720 horas.&#x20;

<figure><img src="../../.gitbook/assets/image (568).png" alt=""><figcaption><p>Elementos de Gestión de Campañas</p></figcaption></figure>

**Ejemplo:** En este caso, dado que ninguna solicitud ha alcanzado la marca de las primeras 1000, no se aplicarán cargos por las acciones realizadas en la página de campañas. Sin embargo, dado que había campañas en ejecución o listadas, se cobraron un total de 2201,09 horas de campaña, lo que equivale a unas 3 campañas en ejecución durante todo un mes. Esto dio lugar a un coste total de 2,29 $. Tenga en cuenta que las campañas se cobran por estar listadas, estén activas o no, por lo que al eliminar una campaña se detendrán los cargos adicionales.

{% hint style="info" %}
Todos los productos generan métricas una vez que se empiezan a utilizar. Estas métricas se cobran y son cruciales para comprender el uso y el rendimiento de su plataforma BMS. El [Pestaña de Monitoreo](../monitoring/monitoring-billing.md#metric-monitoring) es responsable de estas métricas y mostrará la factura correspondiente.\
BMS se centra en la transparencia y le mostrará los costes de todas las funciones de cada producto.
{% endhint %}
