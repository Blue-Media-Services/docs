# Grupos de Criativos

Grupos de Criativos permitem que você agrupe vários criativos como uma única unidade. Você pode então aplicar pesos diferentes a cada um e, posteriormente, verificar o desempenho de um em relação aos outros.

Eles são muito úteis se você deseja exibir diversas variações dos mesmos banners, mantendo uma configuração simples para os Anúncios. É também como você pode realizar [testes A/B](creative-groups.md#a-b-testing) para determinar quais criativos têm o melhor desempenho.

## Gerenciandos Grupos de Criativos <a href="#managing-creative-groups" id="managing-creative-groups"></a>

<figure><img src="../../.gitbook/assets/image (218).png" alt=""><figcaption><p>Lista de Grupos de Criativos</p></figcaption></figure>

### Criando um Grupo de Criativos <a href="#creating-a-creative-group" id="creating-a-creative-group"></a>

Na página de Grupos de Criativos, clique em <img src="../../.gitbook/assets/image (558).png" alt="Create Creative Group" data-size="line">.

Preencha as informações:

<figure><img src="../../.gitbook/assets/image (717).png" alt=""><figcaption><p>Editor de Grupo de Criativos</p></figcaption></figure>

* Nome - como você deseja chamar este grupo de criativos;
* Tags - até 5 rótulos que podem ser usados para auxiliar na identificação e busca;
* Domínio - este é o domínio principal para o qual os criativos neste grupo levarão o usuário ao serem clicados;
* Tipo - o tipo de criativo, pode ser qualquer tamanho IAB comum como "Large Leaderboard (970x90)", "Banner (468x60)", etc.

Configure a composição do grupo de criativos:

<figure><img src="../../.gitbook/assets/image (220).png" alt=""><figcaption><p>Composição do Grupo de Criativos</p></figcaption></figure>

Selecione pelo menos um criativo para fazer parte deste grupo. Para adicionar mais criativos, use o botão <img src="../../.gitbook/assets/add.png" alt="Add" data-size="line">. Para remover um criativo existente, use o botão <img src="../../.gitbook/assets/remove.png" alt="Remove" data-size="line">.

Você pode criar um novo criativo diretamente deste editor clicando no botão <img src="../../.gitbook/assets/create.png" alt="Create" data-size="line">, ou pode editar um criativo existente clicando em <img src="../../.gitbook/assets/edit.png" alt="Edit" data-size="line">.

Por padrão, o sistema atribuirá peso igual a todos os criativos. Se você deseja direcionar mais tráfego para um criativo em detrimento de outro, simplesmente ajuste a coluna de pesos. O sistema calculará a proporção aproximada de impressões que cada um terá.

Clique no botão <img src="../../.gitbook/assets/image (221).png" alt="Preview Group" data-size="line"> para ver uma pré-visualização deste grupo:

<figure><img src="../../.gitbook/assets/image (222).png" alt=""><figcaption><p>Prévia do Grupo de Criativos</p></figcaption></figure>

Após fazer todas as alterações necessárias, clique em <img src="../../.gitbook/assets/image (561).png" alt="Save" data-size="line">.

### Editando um Grupo de Criativos <a href="#editing-a-creative-group" id="editing-a-creative-group"></a>

Para editar um grupo de criativos, use o botão <img src="../../.gitbook/assets/edit.png" alt="Edit" data-size="line"> na lista de grupos de criativos. Todos os campos estão disponíveis para edição, exceto os seletores de domínio e tipo.

<figure><img src="../../.gitbook/assets/image (560).png" alt=""><figcaption><p>Editando um Grupo de Criativos</p></figcaption></figure>

Depois de fazer as alterações necessárias em seu grupo de criativos, clique em <img src="../../.gitbook/assets/image (561).png" alt="Save" data-size="line">.

### Verificando o status de um Grupo de Criativos <a href="#checking-the-status-of-a-creative-group" id="checking-the-status-of-a-creative-group"></a>

Na lista de Grupos de Criativos, ao passar o mouse sobre o sinal de aviso, você pode verificar o status do seu criativo.

<figure><img src="../../.gitbook/assets/image (242).png" alt=""><figcaption><p>Grupo de Criativos com Problema</p></figcaption></figure>

Assim que todos os problemas forem resolvidos, o grupo de criativos exibirá o sinal <img src="../../.gitbook/assets/image (562).png" alt="Check" data-size="line">.

### Arquivando e Desarquivando um Grupo de Criativos <a href="#archiving-and-unarchiving-a-creative-group" id="archiving-and-unarchiving-a-creative-group"></a>

Grupos de Criativos que não estão sendo usados com frequência podem ser arquivados clicando no botão <img src="../../.gitbook/assets/archive.png" alt="Archive" data-size="line">. Arquivar um grupo de criativos não impede que ele seja usado ou exibido, apenas o oculta da visualização principal.

Para ver todos os grupos de criativos arquivados, simplesmente ative o filtro <img src="../../.gitbook/assets/archive filter.png" alt="Archived" data-size="line"> filter. . Você pode desarquivar <img src="../../.gitbook/assets/image (18).png" alt="" data-size="line"> um criativo para movê-lo para a visualização principal.

### Excluindo um Grupo de Criativos <a href="#deleting-a-creative-group" id="deleting-a-creative-group"></a>

Você pode excluir um grupo de criativos clicando em <img src="../../.gitbook/assets/delete.png" alt="Delete" data-size="line">. Se o grupo de criativos estiver sendo usado, você verá uma lista de anúncios que serão afetados. Se você confirmar a exclusão, os anúncios serão modificados para remover o grupo de criativos excluído da rotação.

<figure><img src="../../.gitbook/assets/image (226).png" alt=""><figcaption><p>Confirmação de exclusão mostrando grupo de criativos em uso</p></figcaption></figure>

{% hint style="danger" %}
Atenção! Se você excluir um grupo de criativos, todos os dados relacionados a esse grupo, incluindo métricas coletadas anteriormente, também serão excluídos. Esta ação não pode ser desfeita.
{% endhint %}

## Monitorando Grupos de Criativos <a href="#monitoring-creative-groups" id="monitoring-creative-groups"></a>

### Aba de Métricas <a href="#metrics-tab" id="metrics-tab"></a>

A aba de métricas exibirá todas as métricas relacionadas aos criativos selecionados ou para toda a conta, se nenhum criativo for selecionado. Encontre abaixo todas as métricas disponíveis para seus grupos de criativos.

* [Entregas](ad-server-metrics.md#entregas-e-taxa-de-entrega)
* [Exibições e Taxa de Exibição](ad-server-metrics.md#exibicoes-e-taxa-de-exibicao)
* [Visualizações](ad-server-metrics.md#visualizacoes)
* [Visibilidade](ad-server-metrics.md#visibilidade)
* [Cliques e CTR](ad-server-metrics.md#cliques-e-ctr)
* [Taxa de Clique para Carregamento de Página](ad-server-metrics.md#taxa-de-clique-para-carregamento-de-pagina)
* [Tempo até a Exibição](ad-server-metrics.md#tempo-ate-a-exibicao)
* [Tempo até a Visualização](ad-server-metrics.md#tempo-ate-a-visualizacao)
* [Tempo até o Clique](ad-server-metrics.md#tempo-ate-o-clique)
* [Tempo para Carregamento de Página](ad-server-metrics.md#tempo-para-carregamento-da-pagina)
* [Carregamentos de Página](ad-server-metrics.md#carregamentos-de-pagina)
* [Taxa de Carregamento de Página](ad-server-metrics.md#taxa-de-carregamento-de-pagina)

#### Teste A/B <a href="#a-b-testing" id="a-b-testing"></a>

Para verificar o desempenho dos criativos em um grupo, selecione o grupo desejado na lista e, em seguida, altere as métricas para serem agrupadas por **Criativo** em vez de por **Grupo de Criativos**. Assim, você poderá comparar qualquer uma das métricas disponíveis entre os criativos que estão sendo testados no grupo.

<figure><img src="../../.gitbook/assets/image (243).png" alt=""><figcaption><p>Métricas apresentando resultados de um Teste A/B</p></figcaption></figure>

### Aba de Tempo Real <a href="#real-time-tab" id="real-time-tab"></a>

A aba de tempo real exibirá eventos em tempo real relacionados ao grupo de criativos selecionado.

Saiba mais sobre a [Aba de Tempo Real](../demand-side-platform-dsp/real-time-tab.md).
