# Identifier Pools

Identifier pools funciona de manera muy similar a cookie pools pero están diseñados específicamente para dispositivos móviles, incluidos teléfonos inteligentes Android, tabletas y productos iOS. Cada sistema operativo emplea sus propios métodos únicos para identificar a los usuarios de manera eficaz.

Android de Google utiliza el GAID (Google Advertising ID), un identificador único proporcionado por Google Play Services con fines publicitarios. El GAID permite a los desarrolladores y anunciantes realizar un seguimiento de la actividad de los usuarios y ofrecer anuncios personalizados, al tiempo que proporciona a los usuarios control sobre su configuración de privacidad.

El sistema operativo iOS de Apple asigna un identificador único y aleatorio a cada usuario, conocido como IDFA (Identificador para anunciantes). Al igual que el GAID, el IDFA permite a los desarrolladores y anunciantes supervisar la actividad de los usuarios y ofrecerles anuncios personalizados, al tiempo que ofrece a los usuarios control sobre sus preferencias de privacidad.

## Gestión de Identifier Pools

<figure><img src="../../.gitbook/assets/image (470).png" alt=""><figcaption><p>Lista de Identifier Pools</p></figcaption></figure>

### Crear un Identifier Pool

Un Identifier Pool debe crearse antes de utilizarse para una campaña, de modo que pueda rellenarse. Configure cuánto tiempo deben estar disponibles los identificadores antes de caducar y establezca cuántos identificadores desea almacenar en su pool. Además, seleccione un Ad Exchange para sincronizar tus identificadores con él.

1. Haga clic en ![Create Identifier Pool](<../../.gitbook/assets/image (475).png>) para crear un nuevo identifier pool.
2.  Rellene los datos:

    <figure><img src="../../.gitbook/assets/image (473).png" alt=""><figcaption><p>Editor de Identifier Pool</p></figcaption></figure>

    * Nombre: Indique cómo desea nombrar su identifier pool.
    * Etiquetas: Establece etiquetas para organizar tu identifier pools.
    * Exchanges: Seleccione el deseado Ad Exchanges.
    * TTL: Establezca el número de días que desea mantener los identificadores en el pool después de añadir.
    * Tamaño máximo: Defina cuántos identificadores se pueden añadir al pool.
3. Haga clic en ![Save](<../../.gitbook/assets/image (476).png>) para guardar tu Identifier Pool.

### Editar un Identifier Pool

Después de crear un identifier pool, puedes editarlo haciendo clic en el botón de edición ![Edit](<../../.gitbook/assets/image (482).png>). Todos los parámetros son editables. En el caso del TTL, los cambios solo se aplicarán a los identificadores recién añadidos. Después de realizar los cambios, haga clic en ![Save](<../../.gitbook/assets/image (476).png>) para salvarlos.

Es posible archivar identifier pools para una mejor organización. Haga clic en ![Archive](<../../.gitbook/assets/image (1067).png>) para archivar los seleccionados identifier pools, y visualizar sus archivos archivados identifier pools activando el interruptor "Archivado" situado encima del identifier pools lista. También es posible desarchivar un identifier pool haciendo clic en ![Unarchive](<../../.gitbook/assets/image (1068).png>).

### Eliminar un Identifier Pool

Puedes eliminar un identifier pool haciendo clic en el botón eliminar ![Delete](<../../.gitbook/assets/image (1070).png>), para continuar con el proceso, haga clic en ![Delete](<../../.gitbook/assets/image (1071).png>) para confirmar. Tenga en cuenta que las acciones del rastreador basadas en estas identifier pools dejará de funcionar.

{% hint style="danger" %}
¡Atención! Ten cuidado al eliminar identifier pools, esta acción no se puede deshacer y todos los datos relacionados, incluidas las métricas recopiladas anteriormente, también se eliminarán.
{% endhint %}

## Configuración de Identifier Pools

Después de crear un Identifier Pool, es necesario configurarlo antes de utilizarlo como objetivo en una campaña.

Para utilizar los Identifier Pools, deberá configurar un rastreador o utilizar uno ya existente. Este artículo está dedicado a la función de Identifier Pools. Acceda a nuestro [Rastreadores](trackers/) documentación para obtener más información sobre cómo configurar un rastreador.

### Crear una Acción Vinculada a un Identifier Pool

Siga los pasos que se indican a continuación para crear una acción para un rastreador que añadirá o eliminará usuarios de su identifier pools.

Después de crear y seleccionar un rastreador de la lista de rastreadores, siga los pasos que se indican a continuación para vincularlo a su identifier pool:

1. En la pestaña Configuración, en la sección de eventos rastreados, haga clic en ![Add Event](<../../.gitbook/assets/image (485).png>) para añadir un nuevo evento.
2.  Rellene los datos:

    <figure><img src="../../.gitbook/assets/image (488).png" alt=""><figcaption><p>Editor de eventos</p></figcaption></figure>

    * Nombre: Indique cómo desea nombrar este evento.
    * ID del evento: Este campo se puede personalizar para establecer un ID de evento diferente; sin embargo, se rellena automáticamente con el nombre del evento.
    * Campos de datos personalizados: Establezca los campos de datos que se recopilarán cuando se capture el evento.
    * Acciones: Establezca las acciones que se ejecutarán cuando se solicite este evento. En este artículo, estableceremos una acción que añade o elimina identificadores de nuestro identifiers pool.
    *
      1. Haga clic en ![Add Event](<../../.gitbook/assets/image (485).png>) para añadir una nueva acción.
      2.  Rellene los datos:

          <figure><img src="../../.gitbook/assets/Captura de tela 2025-02-27 084528.png" alt=""><figcaption><p>Editor de Acciones</p></figcaption></figure>

          1. Nombre: Establezca un nombre para su evento.
          2. Seleccionar rastreador en Identifier Pool
          3. Identifier Pool: Seleccione el identifier pool te enlazarás con esta acción.
          4. Seguir como: Seleccione esta opción si desea añadir o eliminar identificadores del pool.
          5. Haga clic en ![Save](<../../.gitbook/assets/image (476).png>) para guardar tu acción.
3. Haga clic en ![Save](<../../.gitbook/assets/image (476).png>) de nuevo para guardar tu evento.

El rastreador debe instalarse en todas las páginas de su sitio web en las que desee realizar un seguimiento de la actividad de los usuarios. Tras instalar el rastreador, es posible que el sistema tarde un tiempo, dependiendo del tráfico de su sitio web, en recopilar suficientes identificadores para utilizarlo como objetivo en una campaña.

## Pestaña Métricas

Puedes seguir tu Identifier Pools a medida que crecen, esto se puede hacer utilizando la pestaña de métricas de la Identifiers Pool página. Estas son todas las métricas para esta función:

* [Recuento de Identifiers Añadidos](dmp-metrics.md#identifiers-added-count)
* [Recuento de Identifiers Habilitados](dmp-metrics.md#identifiers-enabled-count)
* [Recuento de Identifiers Caducados](dmp-metrics.md#identifiers-expired-count)
* [Recuento de Identifiers Eliminados Manualmente](dmp-metrics.md#identifiers-manually-removed-count)
* [Tamaño Máximo](dmp-metrics.md#max-size-1)
* [Tamaño](dmp-metrics.md#size-1)
* [Tiempo hasta el Vencimiento](dmp-metrics.md#time-until-expiration-2)
