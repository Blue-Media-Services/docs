# Looker Studio

Looker Studio es una plataforma de inteligencia empresarial y visualización de datos que permite a los usuarios transformar datos sin procesar en informes personalizados. Se integra con múltiples fuentes de datos, lo que permite a los usuarios crear paneles de control en tiempo real para realizar un seguimiento del rendimiento y analizar datos.

{% hint style="warning" %}
_¡Atención! Antes de continuar, es necesario crear una Clave API con permiso para leer los datos métricos de su cuenta. Puede aprender cómo hacerlo en nuestro_ [_Claves API_](../product-documentation/gestion-de-acceso-e-identidad-iam/api-keys.md) _artículo._
{% endhint %}

## Conectando BMS con Looker Studio

Si aún no tienes una cuenta BMS, regístrate [aquí](https://console.bluems.com/#signUp).

BMS tiene un conector asociado en Looker Studio para la API de métricas. Este conector le permite enviar datos de sus campañas de BMS a un informe personalizado en Looker Studio. A continuación se indican los pasos para configurar BMS como fuente de datos.

<figure><img src="../.gitbook/assets/image (1024).png" alt=""><figcaption><p>Página de inicio de Looker Studio</p></figcaption></figure>

1. Accede a Looker Studio. Es posible que tengas que crear una cuenta si aún no tienes una.
2. Vaya a la pestaña Fuentes de datos, situada justo debajo de la barra de búsqueda.
3. Haga clic en "+ Crear nueva fuente de datos".
4. Para cambiar el nombre de tu fuente de datos, haz clic en el nombre predeterminado en la esquina superior izquierda de la página.
5.  Busca "BMS" en la barra de búsqueda.

    <figure><img src="../.gitbook/assets/image (1025).png" alt=""><figcaption><p>Encontrar el conector BMS</p></figcaption></figure>
6. Haga clic en BMS Monitoring para seleccionarlo como fuente de datos.
7.  Rellene con los parámetros correctos:

    <figure><img src="../.gitbook/assets/image (1026).png" alt=""><figcaption><p>Parámetros del conector BMS</p></figcaption></figure>

    * **ID de Cuenta BMS:** Introduzca el ID de cuenta BMS de la cuenta que va a conectar a Looker Studio, utilizando el formato XXXX-XXXX-XXXX.
    * **Clave API BMS:** Proporcione un código secreto de Clave API BMS con permiso para leer los datos métricos de su cuenta BMS.
    * **Período de Agregación:** Defina el intervalo de tiempo predeterminado para agregar estadísticas métricas al consultar datos por marcas de tiempo.
    * **Desfase Horario:** Establezca el desfase UTC para determinar el inicio de un día al agrupar datos por día.
    * **Permitir que se modifique el "Período de agregación" en los informes:** Marque esta opción si desea permitir que se modifique el período de agregación en los informes.
8. Después de completar todos los parámetros correctamente, haga clic en "Conectar" en la esquina superior derecha de la página para completar la conexión.

## Información Adicional

Ahora los datos métricos de su cuenta BMS están disponibles como fuente de datos para los informes de Looker Studio. Puede utilizarlos para crear informes personalizados que le proporcionarán valiosa información empresarial. A continuación, le ofrecemos algunos artículos de Looker Studio que le ayudarán en este proceso:

* [Crear un informe](https://cloud.google.com/looker/docs/studio/create-a-report)
* [Acerca de los conectores, las fuentes de datos y las credenciales](https://cloud.google.com/looker/docs/studio/about-connectors-data-sources-and-credentials)
* [Nuestra Política de Privacidad](https://bluems.com/privacy/home.html)
* [Nuestras Condiciones de Uso](https://console.bluems.com/assets/docs/signup-terms-and-conditions-20240404.pdf)
