# Sincronización Externa de Data Lake (AWS)

La integración entre Almacenes de Eventos y AWS permite la transferencia fluida de datos de eventos a un bucket S3, lo que garantiza un archivado, una copia de seguridad y una accesibilidad eficientes de los datos. Exportar sus datos a un lago de datos externo le proporciona un mayor control sobre ellos, lo que le permite obtener información valiosa.

{% hint style="warning" %}
Antes de comenzar, asegúrese de tener acceso a la consola de administración de AWS con permisos para administrar nubes privadas virtuales (VPC), grupos de seguridad, funciones Lambda y roles de IAM. Además, tenga en cuenta que este procedimiento puede generar costos adicionales en su cuenta de AWS debido a la creación y el uso de nuevos recursos.
{% endhint %}

## Implementación de Infraestructura con AWS CloudFormation

Se han desarrollado dos plantillas utilizando CloudFormation para optimizar la configuración de la integración y proporcionar la infraestructura mínima necesaria. Dependiendo de sus conocimientos técnicos, puede personalizar estas plantillas después de su configuración inicial para adaptarlas a las necesidades de su empresa.

{% hint style="info" %}
Para continuar, necesita una clave API creada con permisos de solo lectura para los almacenes de eventos. Puede aprender a crear y recuperar una clave API en este [artículo](../product-documentation/gestion-de-acceso-e-identidad-iam/api-keys.md).
{% endhint %}

### Plantilla con VPC

Utilice esta plantilla si ya tiene configurada una nube privada virtual (VPC) en su cuenta de AWS. Acceda a la plantilla [aquí](https://us-east-2.console.aws.amazon.com/cloudformation/home?region=us-east-2#/stacks/quickcreate?templateUrl=https://bms--public-files.s3.us-east-1.amazonaws.com/with-vpc.yaml\&stackName=bms%E2%80%93monitoring%E2%80%93event-pipe%E2%80%93event-recorder).

<figure><img src="../.gitbook/assets/image (1037).png" alt=""><figcaption><p>Plantilla con VPC</p></figcaption></figure>

Después de acceder a la plantilla, rellene los datos:

* Nombre de la Pila: Este campo se rellena automáticamente, pero puede utilizarlo para personalizar el nombre de la pila.
* Nombre del Bucket S3: Indique o cree un nombre para su bucket S3.
* Crear Bucket S3: Seleccione 'true' para crear un nuevo bucket S3 o 'false' para utilizar uno existente.
* ID de Cuenta: Indique su ID de cuenta BMS.
* ID del Almacén de Eventos: Indique el ID del almacén de eventos, que puede encontrar haciendo clic en <img src="../.gitbook/assets/image (1035).png" alt="edit" data-size="line"> en la misma fila que el almacén de eventos que desea importar.
* Clave API: Indique una clave API BMS con la política de acceso "MON - Almacenes de eventos - Read Only" (MON - Almacenes de eventos - Solo lectura).

Después de rellenar todos los campos, al final de la página, debe aceptar que AWS CloudFormation pueda crear recursos IAM para esta plantilla. A continuación, haga clic en "Crear pila" para continuar con la creación de la pila.

### Plantilla sin VPC

Si su cuenta de AWS no tiene configurada una nube privada virtual (VPC), utilice esta plantilla, a la que se puede acceder [aquí](https://us-east-2.console.aws.amazon.com/cloudformation/home?region=us-east-2#/stacks/quickcreate?templateUrl=https://bms--public-files.s3.us-east-1.amazonaws.com/without-vpc.yaml\&stackName=bms%E2%80%93monitoring%E2%80%93event-pipe%E2%80%93event-recorder).

<figure><img src="../.gitbook/assets/image (1038).png" alt=""><figcaption><p>Plantilla sin VPC</p></figcaption></figure>

Después de acceder a la plantilla, rellene los datos:

* Nombre de la Pila: Este campo se rellena automáticamente, pero puede utilizarlo para personalizar el nombre de la pila.
* Nombre del Bucket S3: Indique o cree un nombre para su bucket S3.
* Crear Bucket S3: Seleccione 'true' para crear un nuevo bucket S3 o 'false' para utilizar uno ya existente.
* ID de Cuenta: Indique su ID de cuenta BMS.
* ID de Almacén de Eventos: Indique el ID de almacén de eventos, que puede encontrar haciendo clic en <img src="../.gitbook/assets/image (1035).png" alt="edit" data-size="line"> en la misma fila que el almacén de eventos que desea importar.
* Clave API: Indique una clave API BMS con la política de acceso "MON - Almacenes de eventos - Read Only" (MON - Almacenes de eventos - Solo lectura).
* ID de Subred: Seleccione una ID de subred para la función Lambda en la lista desplegable.
* ID de grupo de Seguridad: Seleccione una ID de grupo de seguridad para la función Lambda en la lista desplegable.

Después de rellenar todos los campos, al final de la página, debe aceptar que AWS CloudFormation pueda crear recursos IAM para esta plantilla. A continuación, haga clic en 'Crear pila' para continuar con la creación de la pila.

## Información Adicional

Ahora que ha integrado sus almacenes de eventos BMS con AWS y sus datos comenzarán a enviarse tan pronto como se complete la creación de la pila, puede seguir este proceso en el panel de control de sus pilas. Consulte estos artículos para obtener más información sobre las funciones relacionadas con BMS y los productos de AWS:

* [Pipelines de Eventos](../product-documentation/monitoring/event-pipes.md)
* [Almacenamiento de Eventos](../product-documentation/monitoring/event-stores.md)
* [Claves API](../product-documentation/gestion-de-acceso-e-identidad-iam/api-keys.md)
* [AWS CloudFormation](https://docs.aws.amazon.com/cloudformation/)
