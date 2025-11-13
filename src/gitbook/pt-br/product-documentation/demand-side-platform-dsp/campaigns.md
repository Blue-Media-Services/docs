---
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

# Gerenciando Campanhas

## Criando uma Campanha <a href="#creating-a-campaign" id="creating-a-campaign"></a>

Na tela de Campanhas, clique em <img src="../../.gitbook/assets/image (761).png" alt="Create Campaign" data-size="line">.

Preencha as informações:

<figure><img src="../../.gitbook/assets/image (747).png" alt=""><figcaption><p>Criação de Campanha</p></figcaption></figure>

* Nome - Escolha um nome para sua campanha;
* Tags - Até 5 rótulos que podem ser usados para auxiliar na identificação e busca;
* Domínio - Este é o domínio principal para o qual esta campanha levará o usuário ao ser clicado;
* Fuso Horário – Em qual fuso horário você deseja veicular sua campanha;
* Agendamento - Defina a data de início e término para a Campanha;
* Preço do Lance – É aqui que você decidirá seu preço de lance para o leilão de anúncios;
  * Fixo - Defina seu preço imutável para um espaço de inventário;
  * Variável - Ative esta opção para usar nossa tecnologia "_**Bid Shading**_", que é o sistema de lances da própria plataforma; se ativado, ele otimizará o gasto do seu orçamento, sempre focando no valor mais justo para a compra desses espaços de inventário. Isso gera uma economia significativa, embora a empresa possa optar por não ativar o _Bid Shading_ e deixar que a oferta do lance seja baseada apenas na meta de CPM.
* Limite de Frequência: Quantidade de impressões por dispositivo. Aqui você pode alterar quantas vezes a campanha será mostrada para cada dispositivo;

{% hint style="warning" %}
Atenção! Quanto maior o Limite de Frequência, mais você aparecerá para o mesmo usuário. Quanto menor o Limite de Frequência, você alcançará mais usuários e aparecerá com menos frequência para cada um deles.
{% endhint %}

Após preencher todos os campos, clique em ![](<../../.gitbook/assets/image (762).png>). Se houver algum campo inválido, ele será mostrado para que você possa revisar o que está faltando.

Esta será sua visualização após criar uma campanha com sucesso.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-12-05 073504.png" alt=""><figcaption><p>Lista de Campanhas</p></figcaption></figure>

## Configurando sua Campanha <a href="#configuring-your-campaign" id="configuring-your-campaign"></a>

Para começar a configurar sua Campanha, marque a <img src="../../.gitbook/assets/image (35).png" alt="" data-size="line"> da campanha desejada e a aba de configuração será exibida.

<figure><img src="../../.gitbook/assets/image (1080).png" alt=""><figcaption><p>Configuração de Campanha </p></figcaption></figure>

Configure seu [Orçamento](budgets.md), [Públicos-alvo](targets.md) e [Anúncios](managing-ads.md).

## Habilitando sua Campanha <a href="#enabling-your-campaign" id="enabling-your-campaign"></a>

Para habilitar sua campanha, você deve ter pelo menos um Público-alvo e um Anúncio adicionados à campanha. Você também pode verificar o sinal de <img src="../../.gitbook/assets/image (463).png" alt="" data-size="line"> para ver se há algum problema impedindo a ativação da campanha.

{% hint style="warning" %}
Se este aviso aparecer no status do seu criativo, anúncio ou campanha, significa que o material não foi aprovado pela plataforma ou pelas _ad exchanges_. Nesse caso, a BMS informará o problema em questão (em detalhes) ao passar o cursor sobre o sinal, e você poderá fazer os ajustes necessários antes da ativação.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (1081).png" alt=""><figcaption><p>Campanha</p></figcaption></figure>

Para habilitar sua campanha, acione o botão Habilitar.

<div align="center"><figure><img src="../../.gitbook/assets/image (156).png" alt="" width="269"><figcaption><p>Campanha Habilitada</p></figcaption></figure></div>

## Duplicando sua Campanha <a href="#duplicating-your-campaign" id="duplicating-your-campaign"></a>

Se você deseja reutilizar uma campanha com diferentes configurações sem ter que criar uma nova do zero, tem a opção de duplicar uma campanha. Clique em <img src="../../.gitbook/assets/image (36).png" alt="" data-size="line"> na campanha que deseja duplicar e uma cópia dessa campanha será listada. Ao duplicar uma campanha, você também duplica anúncios, orçamento e públicos-alvo.

## Arquivando e Desarquivando sua Campanha <a href="#archiving-and-unarchiving-your-campaign" id="archiving-and-unarchiving-your-campaign"></a>

Se uma campanha já cumpriu seu propósito, mas você não deseja excluí-la, tem a opção de arquivá-la. Clique em <img src="../../.gitbook/assets/image (37).png" alt="" data-size="line"> para arquivar.

Para verificar suas campanhas arquivadas, clique em <img src="../../.gitbook/assets/image (38).png" alt="" data-size="line"> para mudar sua visualização para campanhas Arquivadas. Lá você verá todas elas e, se desejar recuperar uma campanha, basta clicar em <img src="../../.gitbook/assets/image (39).png" alt="" data-size="line"> e a campanha estará disponível novamente.

## Excluindo uma Campanha <a href="#deleting-a-campaign" id="deleting-a-campaign"></a>

Se precisar excluir uma campanha, basta clicar em <img src="../../.gitbook/assets/image (40).png" alt="" data-size="line"> e uma tela de confirmação será exibida. Esta ação não pode ser desfeita e você terá que digitar manualmente o nome da campanha para excluí-la.

<figure><img src="../../.gitbook/assets/image (198).png" alt=""><figcaption><p>Tela de Exclusão de Campanha</p></figcaption></figure>

{% hint style="danger" %}
_Atenção! Aconselhamos sempre a desativar a campanha em vez de excluí-la completamente. Ao excluir uma campanha, todos os dados e métricas também são perdidos._
{% endhint %}

## Aba de Métricas <a href="#metrics-tab" id="metrics-tab"></a>

Enquanto os eventos em tempo real são mantidos por 15 minutos, você pode verificar as métricas da campanha para qualquer intervalo de tempo. As métricas podem levar até 5 minutos para exibir os dados mais recentes. Abaixo você encontra todas as métricas disponíveis para sua Campanha.

* [Campanha Ativa](dsp-metrics.md#campanha-ativa)
* [Orçamento Gasto](dsp-metrics.md#orcamento-gasto)
* [Lances e Taxa de Lances Ganhos](dsp-metrics.md#lances-e-taxa-de-lances-ganhos)
* [Impressões](dsp-metrics.md#impressoes)
* [Preço da Impressão](dsp-metrics.md#preco-da-impressao)
* [CPM](dsp-metrics.md#cpm)
* [CPC](dsp-metrics.md#cpc)
* [Entregas e Taxa de Entrega](../ad-server/ad-server-metrics.md#entregas-e-taxa-de-entrega)
* [Exibições e Taxa de Exibição](../ad-server/ad-server-metrics.md#exibicoes-e-taxa-de-exibicao)
* [Visualizações](../ad-server/ad-server-metrics.md#visualizacoes)
* [Visibilidade](../ad-server/ad-server-metrics.md#visibilidade)
* [Duração da Visibilidade e Duração da Exposição](../ad-server/ad-server-metrics.md#duracao-da-visibilidade-e-duracao-da-exposicao)
* [Cliques e CTR](../ad-server/ad-server-metrics.md#cliques-e-ctr)
* [Taxa de Clique para Carregamento de Página](../ad-server/ad-server-metrics.md#taxa-de-clique-para-carregamento-de-pagina)
* [Custo por Carregamento de Página](dsp-metrics.md#custo-por-carregamento-de-pagina)
* [Tempo até a Exibição](../ad-server/ad-server-metrics.md#tempo-ate-a-exibicao)
* [Tempo até a Visualização](../ad-server/ad-server-metrics.md#tempo-ate-a-visualizacao)
* [Tempo até o Clique](../ad-server/ad-server-metrics.md#tempo-ate-o-clique)
* [Tempo para Carregamento de Página](../ad-server/ad-server-metrics.md#tempo-para-carregamento-da-pagina)
* [Carregamentos de Página](../ad-server/ad-server-metrics.md#carregamentos-de-pagina)
* [Taxa de Carregamento de Página](../ad-server/ad-server-metrics.md#taxa-de-carregamento-de-pagina)
* [Preço do Lance Alvo](dsp-metrics.md#preco-do-lance-alvo)
* [Preço do Lance Efetivo](dsp-metrics.md#preco-do-lance-efetivo)
* [Contagem de Dispositivos](dsp-metrics.md#contagem-de-dispositivos)
* [Frequência por Dispositivo](dsp-metrics.md#frequencia-por-dispositivo)
* [Orçamento Gasto com Recomendações](dsp-metrics.md#budget-gasto-com-recomendacoes)
* [Orçamento Gasto Realizando Lances](dsp-metrics.md#budget-gasto-na-realizacao-de-lances)
* [Orçamento Gasto em Impressões](dsp-metrics.md#budget-gasto-em-impressoes)
* [Orçamento Gasto em Entregas](dsp-metrics.md#budget-gasto-em-entregas)
* [Ritmo de Orçamento  Alvo](dsp-metrics.md#ritmo-de-budget-alvo)
* [Ritmo de Orçamento Efetivo](dsp-metrics.md#ritmo-de-budget-efetivo)
* [Orçamento Disponível](dsp-metrics.md#budget-disponivel)
* [Limite de Orçamento Diário](dsp-metrics.md#limite-de-budget-diario)

Você também pode visualizar eventos em Tempo Real de sua Campanha através da nossa [Aba de Tempo Real](real-time-tab.md).
