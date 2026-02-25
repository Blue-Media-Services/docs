# Métricas de DMP

Estas son todas las métricas disponibles en el producto DMP para analizar el rendimiento de sus cookie pools y rastreadores. Además, al revisar las métricas, siempre puede utilizar el <img src="../../.gitbook/assets/image (462).png" alt="" data-size="line"> para acceder a nuestros artículos sobre una métrica específica.

{% hint style="info" %}
Puede obtener más información sobre cómo se gestionan las métricas visitando la página [Métricas](../metricas.md).
{% endhint %}

### **Recuento de Expiración**

Esta métrica muestra cuántas cookies han caducado dentro del intervalo de tiempo configurado. Las cookies caducan en función del TTL, que es el número de días tras los cuales caduca una cookie, configurado al crear la cookie pool.

<figure><img src="../../.gitbook/assets/image (1004).png" alt=""><figcaption><p>Recuento de expiración</p></figcaption></figure>

_**Ejemplo:** Creas un grupo de cookies con un TTL de siete días y lo instalas en tu página de inicio. Las cookies generadas por el acceso de tus usuarios estarán disponibles para la segmentación durante siete días. Transcurrido este periodo, las cookies caducarán. Esto significa que, en una campaña de retargeting, por ejemplo, impactará a los usuarios que hayan visitado su sitio web en los últimos siete días. En este gráfico, puede observar que el 19 de junio caducaron algo menos de 5 cookies, el 20 de junio no caducó ninguna cookie y el 21 de junio caducaron algo menos de 5 cookies, y así sucesivamente._&#x20;

### **Tamaño Máximo**

Esta métrica muestra la cantidad máxima de cookies permitidas en el pool según la configuración.

<figure><img src="../../.gitbook/assets/image (1005).png" alt=""><figcaption><p>Tamaño Máximo</p></figcaption></figure>

_**Ejemplo:** Al crear o editar un cookie pool, puedes establecer la cantidad máxima de cookies en el mismo. Esto limitará el número total de cookies que tu cookie pool puede contener. En este gráfico, puedes observar que se definió un tamaño máximo de 100,000 cookies para este cookie pool._

### **Tamaño**

Esta métrica muestra el tamaño real del cookie pool, lo que significa que mostrará cuántas cookies hay o hubo en el cookie pool dentro del intervalo de tiempo configurado.

<figure><img src="../../.gitbook/assets/image (1006).png" alt=""><figcaption><p>Tamaño</p></figcaption></figure>

_**Ejemplo:** En este gráfico, puede observar el tamaño de un cookie pool en el intervalo de tiempo definido. Esta métrica se puede utilizar para obtener información sobre cuántas cookies se generan dentro del periodo de tiempo configurado, lo que le permitirá establecer un tamaño máximo para el cookie pool que esté en el mismo rango que el número de usuarios en su sitio web._

### **Recuento de Sincronizaciones**

Esta métrica muestra el número de sincronizaciones de cookies, lo que significa que muestra cuándo una cookie recolectada se ha sincronizado con nuestra plataforma y, posteriormente, también con los _exchanges_, lo que le permite segmentar a los usuarios con mayor precisión.

<figure><img src="../../.gitbook/assets/image (1007).png" alt=""><figcaption><p>Recuento de Sincronizaciones</p></figcaption></figure>

_**Ejemplo:** En este gráfico, puede observar el número de sincronizaciones que ocurrieron en un intervalo de tiempo definido. Cuando un usuario accede a su sitio web, se solicitará una cookie para él; después de recibir esta cookie, se analizará si este usuario ya tiene una cookie o no. Si ya la tiene, la nueva cookie se sincronizará con la ya existente, actualizando sus datos en la plataforma; si no la tiene, se creará una cookie para él en la plataforma._

### **Tiempo hasta el Vencimiento**

Esta métrica muestra el tiempo medio restante durante el cual una cookie seguirá estando disponible en el conjunto hasta que caduque en el plazo determinado.

<figure><img src="../../.gitbook/assets/image (1008).png" alt=""><figcaption><p>Tiempo hasta el Vencimiento</p></figcaption></figure>

_**Ejemplo:** Al crear su cookie pool, puede establecer el número de días en los que una cookie expirará; esta métrica le muestra cuánto tiempo queda hasta el vencimiento de una cookie. En este gráfico, el intervalo de tiempo fue de 1 semana, dividido en períodos diarios representados por puntos; puede observar que el 20 de junio quedaba menos de 1 día para que expiraran algunas de las cookies del cookie pool._

### **Recuento de ejecución de Acciones**

Esta métrica muestra cuántas acciones ha ejecutado su rastreador en el periodo de tiempo configurado. También puede agrupar los datos proporcionados por rastreador o por evento, según sus necesidades.

<figure><img src="../../.gitbook/assets/image (450).png" alt=""><figcaption><p>Recuento de ejecución de Acciones</p></figcaption></figure>

_**Ejemplo:** En este gráfico, se puede observar un aumento en el número de acciones a las 6 de la mañana. El gráfico muestra un intervalo de tiempo de 3 horas dividido en intervalos de 5 minutos representados como puntos de datos. Después de crear un rastreador, deberá configurar eventos y acciones. Cada vez que se produzca un evento rastreado, también se ejecutarán las acciones configuradas asociadas a ese evento. Por ejemplo, un evento «añadir al carrito» podría desencadenar una acción para rastrear el producto añadido en el catálogo. Esta métrica indica cuándo y con qué frecuencia se ejecuta la acción dentro de ese intervalo de tiempo._&#x20;

### **Tasa de fracaso de la Acción**

Esta métrica muestra cuándo se ha realizado el seguimiento de un evento, pero la acción vinculada a él ha fallado. También puede agrupar los datos proporcionados por rastreador o por evento, según sus necesidades.

<figure><img src="../../.gitbook/assets/image (451).png" alt=""><figcaption><p>Tasa de fracaso de la Acción</p></figcaption></figure>

_**Ejemplo:** Cuando un usuario añade un producto a su carrito en su sitio web y este evento está configurado para ser rastreado, con una acción para rastrearlo en el catálogo, el evento en sí se rastrea correctamente. Sin embargo, la acción de actualizar el catálogo falló, lo que provocó que el producto no fuera rastreado. En el gráfico, se puede observar que la tasa de fallos de la acción suele ser del 0 %. Sin embargo, hay momentos en los que la tasa de fallos de la acción alcanza picos cercanos al 40 %. El gráfico abarca un periodo de tiempo de 3 horas, dividido en intervalos de 5 minutos representados como puntos de datos._&#x20;

### **Recuento de Actividades**

Cada vez que un usuario realice una actividad rastreada en su sitio web, esta será rastreada. Esta métrica muestra el número de nuevas actividades rastreadas dentro de un periodo de tiempo definido. También puede agrupar los datos proporcionados por rastreador o por evento, según sus necesidades.

<figure><img src="../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>Recuento de Actividades</p></figcaption></figure>

_**Ejemplo:** Tienes un evento "añadir al carrito" configurado en tu rastreador. Cada vez que un usuario añade un producto al carrito, se cuenta como una actividad. En este gráfico, observarás que el número de actividades aumenta después de las 6 de la mañana. También observarás que este gráfico abarca un intervalo de tiempo de 3 horas, dividido en intervalos de 5 minutos representados como puntos de datos._&#x20;

### **Valor de la Actividad**

Algunas actividades rastreadas, como añadir productos al carrito o comprar un producto, pueden tener un valor asociado. Esta métrica representa el valor total de las actividades rastreadas en su sitio web dentro de un periodo de tiempo definido.

<figure><img src="../../.gitbook/assets/image (6) (1).png" alt=""><figcaption><p>Valor de la Actividad</p></figcaption></figure>

_**Ejemplo:** Usted tiene un evento de "compra" (purchase) configurado en su rastreador. Cada vez que un usuario complete una compra, esta métrica se poblará con el valor monetario de dicha transacción. El intervalo de tiempo definido para este gráfico fue de 3 días, dividido en períodos diarios. En el primer período, el valor total de los eventos de compra para este rastreador fue de casi $1,400.00 y, en los días siguientes, este valor disminuyó a casi $300.00._

### **Recuento de Expiración**

Esta métrica muestra el número de caducidades de usuarios que se produjeron en el periodo de tiempo definido.

<figure><img src="../../.gitbook/assets/image (452).png" alt=""><figcaption><p>Recuento de Expiración</p></figcaption></figure>

_**Ejemplo:** Al configurar un rastreador, puede establecer un periodo de seguimiento tras el cual el usuario expirará. Esta métrica muestra el número de expiraciones que ocurrieron. En este gráfico, puede observar que entre las 4 AM y las 5 AM, expiraron casi 50 usuarios rastreados._

### **Usuarios Máximos**

Esta métrica muestra el número máximo configurado de usuarios que se añadirán al rastreador.

<figure><img src="../../.gitbook/assets/image (453).png" alt=""><figcaption><p>Usuarios Máximos</p></figcaption></figure>

_**Ejemplo:** Al crear o editar un rastreador, establecerá el número máximo de usuarios permitidos para ser añadidos a su rastreador. Esta métrica muestra ese dato. En este gráfico, puede observar que el rastreador fue configurado para aceptar hasta 1 millón de usuarios._

### **Tiempo hasta la Expiración**

Esta métrica muestra el tiempo restante que un usuario sigue disponible en el rastreador antes de expirar dentro del intervalo de tiempo determinado.

<figure><img src="../../.gitbook/assets/image (455).png" alt=""><figcaption><p>Tiempo hasta la Expiración</p></figcaption></figure>

_**Ejemplo:** Al crear su rastreador, puede establecer el número de días en los que caducará la actividad rastreada; esta métrica le muestra cuánto tiempo le queda hasta la caducidad de un usuario. En este gráfico, el periodo de tiempo era de una semana, dividida en periodos diarios, representados como puntos. Se puede observar que el 20 de junio quedaba menos de un día para que caducaran algunos de los usuarios del rastreador._&#x20;

### **Recuento de usuarios del Rastreador**

Esta métrica mostrará cuántos usuarios estaban en el rastreador en el intervalo de tiempo definido.

<figure><img src="../../.gitbook/assets/image (456).png" alt=""><figcaption><p>Recuento de usuarios del Rastreador</p></figcaption></figure>

_**Ejemplo:** Después de configurar un rastreador en su sitio web, los usuarios de su sitio comenzarán a ser rastreados. El número de usuarios rastreados dentro de un intervalo de tiempo definido es el dato que muestra esta métrica. En este gráfico, notará que el número de usuarios rastreados entre las 4 AM y las 6 AM fue de casi 400 mil._

### **Recuento de Identifiers Añadidos**

Esta métrica muestra el número total de identificadores añadidos al cookie pool en el intervalo de tiempo definido.

<figure><img src="../../.gitbook/assets/image (463).png" alt=""><figcaption><p>Recuento de Identifiers Añadidos</p></figcaption></figure>

_**Ejemplo:** A medida que los usuarios móviles navegan por las páginas de su sitio web o aplicaciones, en las que ha instalado un rastreador configurado para añadir usuarios a un conjunto de identificadores, estos se irán añadiendo al conjunto. En este gráfico, puede seguir el crecimiento de su grupo de identificadores a medida que se añaden los identificadores de los usuarios. El periodo de tiempo definido fue de una semana, dividida en periodos diarios. Observará que el 31 de diciembre se añadieron algo más de 20 identificadores al grupo y que, en los días siguientes, este número disminuyó a 3 por día, para volver a aumentar a 5 identificadores añadidos el 3 de enero._&#x20;

### **Recuento de Identifiers Habilitados**

Esta métrica muestra el número de identificadores habilitados al menos en un exchange, en el periodo de tiempo definido.

<figure><img src="../../.gitbook/assets/image (464).png" alt=""><figcaption><p>Recuento de Identifiers Habilitados</p></figcaption></figure>

_**Ejemplo:** A medida que los identificadores se añaden a su grupo, la plataforma los enviará a los intercambios publicitarios seleccionados y verificará si están habilitados en sus bases de datos. Este proceso de sincronización puede ser muy útil para las campañas de retargeting._

### **Recuento de Identifiers Caducados**

Esta métrica muestra el número de identificadores del grupo que han caducado en el periodo de tiempo definido.

<figure><img src="../../.gitbook/assets/image (465).png" alt=""><figcaption><p>Recuento de Identifiers Caducados</p></figcaption></figure>

_**Ejemplo:** Creas un grupo de identificadores con un TTL de siete días y lo instalas en tu aplicación. Los identificadores recopilados estarán disponibles para la segmentación durante siete días. Transcurrido este periodo, los identificadores caducarán. Esto significa que, en una campaña de retargeting, por ejemplo, llegarás a los usuarios que hayan utilizado tu aplicación en los últimos siete días. En este gráfico, el periodo de tiempo definido fue de una semana, dividida en periodos diarios. Observará que, desde el 30 de diciembre hasta el 1 de enero, hubo una caducidad al día, luego ninguna caducidad el 2 de enero y, a partir de ahí, volvió a haber una caducidad al día hasta el 5 de enero._&#x20;

### **Recuento de Identifiers eliminados Manualmente**

Esta métrica muestra el número de identificadores eliminados manualmente del grupo en el periodo de tiempo definido.

<figure><img src="../../.gitbook/assets/image (466).png" alt=""><figcaption></figcaption></figure>

_**Ejemplo:** Al configurar un rastreador para un Identifier pool, podrá elegir entre añadir o eliminar identificadores de su grupo. Esta métrica muestra el número de identificadores que se eliminan del grupo mediante este proceso._

### **Tamaño Máximo**

Esta métrica muestra el número máximo de usuarios que el Identifier Pool fue configurado para aceptar en el intervalo de tiempo definido.

<figure><img src="../../.gitbook/assets/image (467).png" alt=""><figcaption><p>Tamaño Máximo</p></figcaption></figure>

_**Ejemplo:** Al crear o editar un identifier pool, puede establecer el número máximo de identificadores que puede contener. Esto limitará el número total de identificadores que su pool puede incluir. En este gráfico, el intervalo de tiempo configurado fue de una semana, dividido en períodos diarios. Notará que el tamaño máximo configurado para este pool no cambió._

### **Tamaño**

Esta métrica muestra el tamaño real del pool, lo que significa que mostrará el número de identificadores que están o estuvieron en el identifier pool dentro del intervalo de tiempo configurado.

<figure><img src="../../.gitbook/assets/image (468).png" alt=""><figcaption><p>Tamaño</p></figcaption></figure>

_**Ejemplo:** En este gráfico, puede observar el tamaño de un identifiers pool en el intervalo de tiempo definido. Esta métrica se puede utilizar para obtener información sobre cuántos identificadores se añaden a su pool dentro del periodo de tiempo configurado, lo que le permitirá establecer un tamaño máximo para el pool que esté en el mismo rango que el número de usuarios en su sitio web. En esta imagen, notará que el 30 de diciembre había 12 usuarios en este pool, en los días siguientes este número disminuyó a 10 usuarios y, el 5 de enero, había 8 usuarios en el pool._

### **Tiempo hasta la Expiración**

Esta métrica muestra la mediana del tiempo restante que un identificador sigue disponible en el pool antes de expirar dentro del intervalo de tiempo determinado.

<figure><img src="../../.gitbook/assets/image (469).png" alt=""><figcaption><p>Tiempo hasta la Expiración</p></figcaption></figure>

_**Ejemplo:** Al crear su identifier pool, puede establecer el número de días en los que un identificador añadido al pool expirará; esta métrica le muestra la mediana del tiempo que tiene hasta el vencimiento de un identificador. En este gráfico, el intervalo de tiempo definido fue de 1 semana, dividido en períodos diarios; notará que el 30 de diciembre la mediana era de alrededor de 16 días hasta que los identificadores expiraran, y en los días siguientes esta mediana siguió aumentando hasta el 5 de enero, cuando se situó en torno a los 23 días para el vencimiento de los identificadores._
