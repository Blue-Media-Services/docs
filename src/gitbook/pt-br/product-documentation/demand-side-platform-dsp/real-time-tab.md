---
description: Learn How our Real Time Tab works.
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Aba de Tempo Real

Os recursos de Anúncio e Campanha possuem uma aba dedicada de monitoramento em tempo real que permite ao cliente ver o que está sendo entregue em tempo real.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-12-30 090101.png" alt=""><figcaption><p>Aba de tempo real mostrando anúncios sendo entregues e interações do usuário enquanto ocorrem</p></figcaption></figure>

Os eventos disponíveis são:

* <img src="../../.gitbook/assets/impression event.png" alt="Impression" data-size="line">\
  Este evento é registrado sempre que uma campanha ganha o direito de exibir um anúncio ao usuário final. Este é o ponto em que o custo de aquisição de mídia é cobrado.
* <img src="../../.gitbook/assets/delivered event.png" alt="Delivered" data-size="line">\
  Este evento é registrado quando o navegador do usuário final solicita o conteúdo do anúncio ao nosso _ad server_. Este é o ponto em que o custo do _ad server_ é cobrado.
* <img src="../../.gitbook/assets/displayed event.png" alt="Displayed" data-size="line">\
  Este evento é registrado quando o navegador do usuário final carrega e exibe o anúncio em uma página.
* <img src="../../.gitbook/assets/viewed event.png" alt="Viewed" data-size="line">\
  Este evento é registrado quando pelo menos 50% do corpo do anúncio é exibido na tela por pelo menos 1 segundo.
* <img src="../../.gitbook/assets/clicked event.png" alt="Clicked" data-size="line">\
  Este evento é registrado quando o usuário final clica no anúncio. Para que este evento seja rastreado, você deve estar usando o Rastreador de Cliques da BMS (_BMS Click Tracker_), que é habilitado por padrão, mas pode ser desabilitado editando o código HTML do criativo.

{% hint style="info" %}
Por favor, note que o evento de impressões (_impression_) só pode ser rastreado para Campanhas e Anúncios.&#x20;

Ao verificar eventos em tempo real para Criativos ou Grupos de Criativos, nenhum evento de "impressão" pode ser registrado. As Regras do Anúncio são determinadas apenas no momento da Entrega do Anúncio. Este é o ponto em que o grupo de criativos final é selecionado e, a partir dele, o criativo final é escolhido.
{% endhint %}

Você pode escolher quais eventos ver alternando o seletor:

<figure><img src="../../.gitbook/assets/image (231).png" alt=""><figcaption><p>Filtro de Eventos</p></figcaption></figure>

Para qualquer evento exibido na lista, você pode clicar no botão de detalhes ![](<../../.gitbook/assets/image (538).png>) para ver mais:

<figure><img src="../../.gitbook/assets/Captura de tela 2024-12-30 090243.png" alt=""><figcaption><p>Tela de Detalhes de Evento</p></figcaption></figure>

Aqui você pode observar todos os detalhes de um evento específico, como a geolocalização do usuário, IP, navegador e tipo de dispositivo. Os parâmetros para o lance (_bid_), _ad exchange_ e domínio, e aqueles relacionados à campanha, público-alvo, anúncio, regra do anúncio, grupo de criativos e criativo específicos, juntamente com uma pré-visualização do próprio criativo.
