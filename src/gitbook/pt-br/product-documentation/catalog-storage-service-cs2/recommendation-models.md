---
description: Learn more about recomendation models and how to create them.
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

# Modelos de Recomendação

Use modelos de recomendação para exibir seus produtos em banners dinâmicos, que mostram produtos diferentes de acordo com quem recebe o anúncio, com a intenção de aumentar suas conversões.

## Gerenciando Modelos de Recomendação <a href="#managing-recommendation-models" id="managing-recommendation-models"></a>

<figure><img src="../../.gitbook/assets/image (350).png" alt=""><figcaption><p>Lista de Modelos de Recomendação</p></figcaption></figure>

### Criando Modelos de Recomendação <a href="#creating-recommendation-models" id="creating-recommendation-models"></a>

Antes de criar um modelo de recomendação, é necessário configurar os catálogos e os serviços da DMP que atuarão como fontes para nossos modelos de recomendação.

1. Clique em <img src="../../.gitbook/assets/image (340).png" alt="" data-size="line"> para começar a criar um modelo de recomendação.
2.  Preencha as informações:<br>

    <figure><img src="../../.gitbook/assets/image (264).png" alt=""><figcaption><p>Editor de Modelos de Recomendação</p></figcaption></figure>

    * Nome: Informe um nome para o seu modelo de recomendação.
    * Tags: Defina tags para sua organização.
    * Catálogo: Selecione o catálogo contendo os produtos que você usará para este modelo de recomendação.
3. Clique em <img src="../../.gitbook/assets/image (341).png" alt="" data-size="line"> para salvar seu modelo de recomendação.

### Configurando Fontes para Modelos de Recomendação <a href="#configuring-recommendation-models" id="configuring-recommendation-models"></a>

Após criar um modelo de recomendação, é necessário configurar suas fontes antes de poder usá-lo. Isso pode ser feito na aba de configuração:

<figure><img src="../../.gitbook/assets/Captura de tela 2024-05-15 095125.png" alt=""><figcaption><p>Aba de Configuração de Modelos de Recomendação</p></figcaption></figure>

1. Selecione um modelo de recomendação na lista.
2. Clique em <img src="../../.gitbook/assets/image (344).png" alt="" data-size="line"> para adicionar uma fonte para este modelo.
3.  Preencha as informações:<br>

    <figure><img src="../../.gitbook/assets/image (338).png" alt=""><figcaption><p>Editor de Fontes de Modelos de Recomendação - Rastreador DMP</p></figcaption></figure>

    * Nome: Informe um nome para sua fonte.
    * Limite: Defina o número máximo de produtos a serem adicionados ao modelo de recomendação por esta fonte.
    * Tipo: Selecione o tipo de fonte que você deseja usar:
      1. Rastreador DMP: Esta opção adicionará produtos ao modelo de recomendação com base nos dados de atividade coletados em seu site.
         * Rastreador: Selecione o rastreador que deseja usar.
         * Evento do _Tracker_ (Rastreador): Selecione o evento rastreado que será considerado para adicionar produtos ao modelo de recomendação.
         * Campo Contendo IDs de Oferta: Informe o campo personalizado que contém o ID da oferta dos produtos que você deseja neste modelo de recomendação.
         * Template: Especifique um _template_ (modelo) para produzir uma lista de IDs de oferta separada por vírgulas para rastrear.
      2.  Ranking de Produtos CS2: Esta opção adicionará produtos ao modelo de recomendação com base na atividade coletada pelo seu catálogo de produtos.

          <figure><img src="../../.gitbook/assets/image (339).png" alt=""><figcaption><p>Editor de Fontes de Modelos de Recomendação - Ranking de Produtos CS2</p></figcaption></figure>

          * Classificar por: Selecione uma atividade classificada entre as opções disponíveis:
            * Mais Adicionados ao Carrinho: Esta opção adicionará os produtos mais adicionados ao carrinho ao seu modelo de recomendação.
            * Mais Pedidos: Esta opção adicionará os produtos mais comprados ao seu modelo de recomendação.
            * Mais Recomendações Clicadas: Esta opção só pode ser usada após executar uma campanha com modelos de recomendação e preencherá seu modelo com os produtos que foram recomendados anteriormente e foram clicados por um usuário.
            * Mais Recomendações Visualizadas: Esta opção só pode ser usada após executar uma campanha com modelos de recomendação e preencherá seu modelo com os produtos que foram recomendados anteriormente e foram visualizados por um usuário.
            * Mais Recomendados: Esta opção só pode ser usada após executar uma campanha com modelos de recomendação e preencherá seu modelo com os produtos mais recomendados.
            * Mais Visualizados: Esta opção adicionará os produtos mais visualizados ao seu modelo de recomendação.
          * No passado: Defina um número de horas no passado para considerar a atividade coletada durante o período para adicionar produtos ao modelo de recomendação.
4. Clique em <img src="../../.gitbook/assets/image (342).png" alt="" data-size="line"> para salvar sua fonte.

Logo após criar sua fonte, uma pré-visualização de seus produtos recomendados estará disponível. Para que esta pré-visualização seja gerada, você deve ter seus cookie pools e rastreadores e/ou os eventos do seu catálogo instalados em seu site, pois seus dados serão usados para gerar as recomendações.

<figure><img src="../../.gitbook/assets/image (384).png" alt=""><figcaption><p>Aba de Configuração de Modelos de Recomendação - Pré-visualização</p></figcaption></figure>

### Editando Modelos de Recomendação e Fontes <a href="#editing-recommendation-models-and-sources" id="editing-recommendation-models-and-sources"></a>

Existem algumas opções de edição disponíveis para modelos de recomendação e fontes.

#### Modelos de Recomendação <a href="#recommendation-models" id="recommendation-models"></a>

Você pode editar o nome e as tags de um modelo de recomendação, no entanto, o catálogo não pode ser alterado. Para fazer esta edição, clique em <img src="../../.gitbook/assets/image (485).png" alt="" data-size="line"> na mesma linha do modelo de recomendação a ser editado.

#### Fontes <a href="#sources" id="sources"></a>

Todos os detalhes da fonte são editáveis. Selecione o modelo de recomendação que contém a fonte a ser editada. Em seguida, na aba de configuração, na seção de fontes, clique em <img src="../../.gitbook/assets/image (486).png" alt="" data-size="line"> na mesma linha da fonte a ser editada, faça suas alterações e clique em <img src="../../.gitbook/assets/image (342).png" alt="" data-size="line"> para salvá-las. Você também pode duplicar uma fonte clicando em <img src="../../.gitbook/assets/image (487).png" alt="" data-size="line">. Isso é útil se você precisar de outra fonte com apenas algumas alterações em comparação com uma existente, mantendo a original.

### **Como as Fontes Funcionam**? <a href="#how-do-sources-work" id="how-do-sources-work"></a>

Fontes são como você coleta dados para alimentar seu Modelo de Recomendação. O Modelo de Recomendação precisa desses dados para organizar os produtos conforme o pretendido. Você deve escolher entre um Rastreador DMP ou um Ranking de Produtos CS2; ambos os métodos funcionam bem, mas cada um requer etapas adicionais para a configuração adequada. Uma vez que você tenha configurado sua fonte corretamente, seu Modelo de Recomendação começará a coletar dados e a se atualizar ativamente, fornecendo ao seu anúncio as informações mais atuais.

### Excluindo Modelos de Recomendação e Fontes <a href="#deleting-recommendation-models-and-sources" id="deleting-recommendation-models-and-sources"></a>

{% hint style="danger" %}
Atenção! Tenha cuidado ao excluir modelos de recomendação. Esta ação não pode ser desfeita e todos os dados relacionados, incluindo métricas coletadas anteriormente, também serão excluídos.
{% endhint %}

Você pode arquivar um modelo de recomendação clicando em <img src="../../.gitbook/assets/image (383).png" alt="" data-size="line"> na mesma linha do modelo que precisa ser arquivado. Também é possível excluir um modelo de recomendação, no entanto, isso excluirá todas as métricas relacionadas a ele. Esta ação não pode ser desfeita, portanto, tenha cuidado ao realizá-la. Clique em <img src="../../.gitbook/assets/image (488).png" alt="" data-size="original"> a mesma linha do modelo de recomendação a ser excluído e confirme a ação clicando em <img src="../../.gitbook/assets/image (489).png" alt="" data-size="line">.

É possível excluir uma fonte. No entanto, isso também excluirá todas as métricas relacionadas a esta fonte, portanto, tenha cuidado ao realizar esta ação. Na seção de fontes da aba de configuração, clique em <img src="../../.gitbook/assets/image (488).png" alt="" data-size="original"> na mesma linha da fonte a ser excluída e confirme a ação clicando em <img src="../../.gitbook/assets/image (489).png" alt="" data-size="line">.&#x20;

## Aba de Métricas <a href="#metrics-tab" id="metrics-tab"></a>

Após configurar seus modelos de recomendação e começar a usá-los em uma campanha, você deve começar a receber dados deles. É possível acompanhar este processo na aba de métricas. Estas são as métricas disponíveis para modelos de recomendação:

* [Contagem de Recomendações de Produto](cs2-metrics.md#contagem-de-recomendacoes-de-produto)&#x20;
* [Contagem de Cliques em Recomendação](cs2-metrics.md#contagem-de-cliques-em-recomendacao)
* [Taxa de Preenchimento de Recomendação](cs2-metrics.md#taxa-de-preenchimento-de-recomendacao)&#x20;
* [Contagem de Requisições de Recomendação](cs2-metrics.md#contagem-de-requisicoes-de-recomendacao)&#x20;
* [Contagem de Visualizações de Recomendação](cs2-metrics.md#contagem-de-visualizacoes-de-recomendacao)
