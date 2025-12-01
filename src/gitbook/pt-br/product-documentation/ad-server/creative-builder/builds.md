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

# Builds

Crie _builds_ com base em seus _blueprints_ para gerar banners dinâmicos para suas campanhas. Banners dinâmicos são úteis porque podem personalizar o que cada usuário vê de acordo com os parâmetros definidos, permitindo campanhas mais envolventes e melhorando os resultados esperados. Por exemplo, ao executar uma campanha de _retargeting_, você pode criar um _build_ para gerar criativos com base em modelos de recomendação, que sugerirão produtos do seu catálogo com base na atividade recente em seu site, melhorando assim suas conversões.

## Gerenciando Builds <a href="#managing-builds" id="managing-builds"></a>

Na página inicial da BMS, clique em Builds, na seção _Ad Server_, para acessar a página de _Builds_.

<figure><img src="../../../.gitbook/assets/image (297).png" alt=""><figcaption><p>Lista de Builds</p></figcaption></figure>

### Criando Builds <a href="#creating-builds" id="creating-builds"></a>

Antes de criar um _build_, é necessário criar seus _blueprints_. Se você ainda não fez isso, siga as instruções na página de [_Blueprints_](blueprints.md) e depois retorne.

1.  Clique em <img src="../../../.gitbook/assets/image (298).png" alt="" data-size="line"> para começar a criar seu _Build_.<br>

    <figure><img src="../../../.gitbook/assets/image (299).png" alt=""><figcaption><p>Editor de Builds</p></figcaption></figure>
2. Preencha os detalhes:
   * Nome: Defina um nome para o seu _Build_.
   * Tags: Defina tags para sua organização.
   * Domínio: Selecione o domínio para o qual você deseja redirecionar o usuário quando ele clicar no anúncio.
   * Blueprint: Selecione o _blueprint_ previamente configurado para começar a configurar seus parâmetros.
   * Tamanhos gerados: Selecione em quais tamanhos os banners de seus anúncios devem ser gerados.
   * Parâmetros: Esta seção mudará de acordo com o _blueprint_ selecionado. Ela conterá os mesmos parâmetros configurados no _blueprint_; você pode ajustar esses parâmetros enquanto observa uma pré-visualização de como seus banners dinâmicos estão sendo gerados.
3. Clique em <img src="../../../.gitbook/assets/image (300).png" alt="" data-size="line"> para salvar seu _Build_.

### Pré-visualizando Banners <a href="#previewing-banners" id="previewing-banners"></a>

A aba Creatives mostra uma pré-visualização de como os banners dinâmicos estão sendo gerados por seus _builds_.

<figure><img src="../../../.gitbook/assets/image (302).png" alt=""><figcaption><p>Aba de Criativos</p></figcaption></figure>

Para ver uma pré-visualização na aba _Criativos_, selecione pelo menos um _build_ da lista de _builds_ marcando a caixa de seleção à esquerda do nome do _build_. Selecionar mais de um mostrará uma pré-visualização de todos os _builds_ selecionados.

### Editando, Arquivando e Excluindo Builds <a href="#editing-archiving-and-deleting-builds" id="editing-archiving-and-deleting-builds"></a>

É possível editar seus _builds_ clicando em <img src="../../../.gitbook/assets/image (30).png" alt="" data-size="line"> na mesma linha do _build_ que você precisa editar. Com exceção do domínio, todos os parâmetros e detalhes estão disponíveis para edição.

Você também pode duplicar _builds_ clicando em <img src="../../../.gitbook/assets/image (31).png" alt="" data-size="line"> na mesma linha do _build_ que precisa duplicar. Isso é útil se você quiser criar um _build_ que altere apenas alguns detalhes em comparação com um existente, mantendo o original.

Arquivar _builds_ é uma opção que ajuda a organizar melhor seus _builds_. Para arquivar um _build_, clique em <img src="../../../.gitbook/assets/image (32).png" alt="" data-size="line"> na mesma linha do _build_ que precisa arquivar. Para visualizar seus _builds_ arquivados, ative a opção "arquivado" acima da lista de _builds_.

Você também pode excluir _builds_. Isso pode ser feito clicando em <img src="../../../.gitbook/assets/image (33).png" alt="" data-size="line"> na mesma linha do _build_ que precisa excluir, selecionando o que deve ser feito com os criativos gerados pelo _build_ e, em seguida, clicando em <img src="../../../.gitbook/assets/image (34).png" alt="" data-size="line"> para confirmar a ação.

{% hint style="danger" %}
Atenção: Tenha cuidado ao excluir _builds_. Esta ação não pode ser desfeita e todos os dados relacionados, incluindo métricas coletadas anteriormente, também serão excluídos.
{% endhint %}

## Métricas dos Builds <a href="#builds-metrics" id="builds-metrics"></a>

{% hint style="info" %}
Você pode aprender mais sobre como as métricas são tratadas visitando a página de [Métricas](../../metrics.md).
{% endhint %}

<figure><img src="../../../.gitbook/assets/Captura de tela 2024-09-13 103846.png" alt=""><figcaption><p>Métricas de Builds</p></figcaption></figure>

As métricas exibidas na aba Métricas da página de _Builds_ são as mesmas da página de Criativos. Para entender como elas funcionam e o que cada uma significa, por favor, verifique nossa página da [Aba de Métricas de Criativos](../creatives.md#aba-de-metricas).
