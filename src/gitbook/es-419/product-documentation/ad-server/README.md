# Ad Server

## Conceptos

### Creativos

Es la unidad básica de nuestro servidor de anuncios. Un creativo representa el código que se entregará al usuario final cuando se muestre su anuncio.&#x20;

Puede proporcionar el código HTML usted mismo o la plataforma puede generarlo por usted si proporciona una imagen y una URL de enlace.&#x20;

Los creativos pueden estar en uno de 3 estados: borrador, en revisión y aprobado. Cualquier modificación al contenido de un creativo lo pondrá en estado de borrador y no se mostrará a los usuarios. Puede enviar cualquier cambio para revisión y, si todo cumple con nuestras políticas, el creativo será aprobado.

### Grupos Creativos

Los grupos de creativos, como su nombre indica, le permiten agrupar varios creativos aplicando diferentes pesos a cada uno.&#x20;

Esto es muy útil al realizar pruebas A/B con cualquier número de creativos para medir cuál funciona mejor.

### Anuncios

Los anuncios son lo que el navegador del usuario final solicita a nuestro servidor de anuncios. Están compuestos por una o más reglas, donde cada regla especifica un conjunto de condiciones que, una vez cumplidas, dirigirán al usuario a un grupo de creativos en particular.&#x20;

Cuando el navegador del usuario realiza la solicitud del anuncio, se entregará el grupo de creativos asociado a la primera regla que coincida. En ese momento, uno de los creativos configurados en el grupo se seleccionará aleatoriamente por peso y se entregará.

### Constructor de Creativos

Para simplificar la creación de creativos estandarizados, puede utilizar Blueprints y Builds. Estas funciones también se pueden usar para generar banners dinámicos que contengan sus productos.

#### Blueprints

Los Blueprints definen un código HTML base que puede generarse dinámicamente según la entrada del usuario. Los parámetros requeridos para la generación también se pueden personalizar.

#### Builds

Cuando tenga un blueprint listo y desee crear creativos a partir de él, crea un build. Un build registrará los tamaños de creativos que desea, el blueprint utilizado y todos los parámetros. Una vez creado, el build generará todos los creativos por usted. Puede alterar cualquier parámetro en cualquier momento y los creativos se actualizarán para reflejar el cambio.
