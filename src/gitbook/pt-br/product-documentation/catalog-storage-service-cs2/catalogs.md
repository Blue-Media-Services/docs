# Catálogos

Na aba Catálogos, você poderá criar um catálogo e, em seguida, instalar um _pixel_ em sua página para que a BMS possa coletar dados com base nos seguintes eventos:

* Produto Visualizado
* Produto Adicionado ao Carrinho
* Produto Comprado

Ao adicionar esses eventos à sua página, poderemos coletar todos os dados necessários para começar a criar métricas e, em seguida, usar nossos **Modelos de Recomendação** para melhorar seus anúncios.

## Gerenciando Catálogos <a href="#managing-catalogs" id="managing-catalogs"></a>

### Criando um Catálogo <a href="#creating-a-catalog" id="creating-a-catalog"></a>

Para criar um catálogo, clique no botão <img src="../../.gitbook/assets/image (127).png" alt="Create Catalog" data-size="line">.

<figure><img src="../../.gitbook/assets/image (128).png" alt="" width="539"><figcaption><p>Tela de Criação de Catálogo</p></figcaption></figure>

Escolha um nome para o seu catálogo e, se desejar, adicione Tags para identificá-lo melhor.

Após preencher os campos, clique em <img src="../../.gitbook/assets/image (129).png" alt="Save" data-size="line">.

Seu catálogo estará então disponível em sua lista.

<figure><img src="../../.gitbook/assets/image (130).png" alt=""><figcaption><p>Lista de Catálogos</p></figcaption></figure>

### Editando um Catálogo <a href="#editing-a-catalog" id="editing-a-catalog"></a>

Se precisar editar o nome ou as tags de um catálogo, clique em <img src="../../.gitbook/assets/image (131).png" alt="Edit" data-size="line">. Após fazer as alterações necessárias, clique em <img src="../../.gitbook/assets/image (132).png" alt="Save" data-size="line">.

### Arquivando um Catálogo <a href="#archiving-a-catalog" id="archiving-a-catalog"></a>

Para arquivar um catálogo, clique em <img src="../../.gitbook/assets/image (133).png" alt="Archive" data-size="line">. Seu catálogo arquivado será então exibido na lista de Arquivado. Para alterar sua visualização, acione a chave seletora <img src="../../.gitbook/assets/image (134).png" alt="Toggle" data-size="line">.

### Desarquivando um Catálogo <a href="#unarchiving-a-catalog" id="unarchiving-a-catalog"></a>

Para desarquivar um catálogo, alterne sua visualização para a lista de Arquivado e clique em <img src="../../.gitbook/assets/image (135).png" alt="Unarchive" data-size="line">. Seu catálogo retornará para a lista de catálogos ativos.

### Excluindo um Catálogo <a href="#deleting-a-catalog" id="deleting-a-catalog"></a>

Para excluir um catálogo, clique em <img src="../../.gitbook/assets/image (136).png" alt="Delete" data-size="line">. Uma tela será exibida para confirmar a exclusão.

<figure><img src="../../.gitbook/assets/image (137).png" alt=""><figcaption><p>Tela de Exclusão de Catálogo</p></figcaption></figure>

Após clicar em <img src="../../.gitbook/assets/image (138).png" alt="Delete" data-size="line">, seu catálogo será **permanentemente** excluído.

{% hint style="danger" %}
Atenção! Aconselhamos desativar o Catálogo em vez de excluí-lo completamente. Ao excluir um Catálogo, todos os dados e métricas também são perdidos.
{% endhint %}

## Instalando Catálogos  <a href="#installing-catalogs" id="installing-catalogs"></a>

Para ativar nossas métricas e eventos, você precisa instalar um _pixel_ em seu site para começar a coletar dados.

Selecione um Catálogo onde deseja instalar seus _pixels_ e, em seguida, vá para a aba Instruções de Instalação.

<figure><img src="../../.gitbook/assets/image (475).png" alt=""><figcaption><p>Aba de Instruções de Instalação</p></figcaption></figure>

Cada evento tem uma página correta para ter seu pixel instalado. Verifique a descrição de cada evento para saber exatamente onde.

{% hint style="info" %}
Lembre-se de substituir a seção pelo seu ID da Oferta (_offer ID_). Cada site tem sua própria maneira de definir uma variável de ID da Oferta, então preste atenção em como essa variável foi configurada em seu site. Se a variável correta não for usada para seus produtos, **o evento não funcionará**. Garanta que a variável de ID da Oferta em seu site retorne os mesmos valores que foram importados como identificadores de produto (em nossa plataforma, eles são chamados de IDs de Oferta) em seu catálogo.
{% endhint %}

_**Exemplo**: O evento de Produto Comprado deve ser instalado em sua **página de confirmação de pedido**._

## Aba de Métricas <a href="#metrics" id="metrics"></a>

Depois de criar seu catálogo e instalar corretamente seus _pixels_, as métricas começarão a ser preenchidas e você poderá rastrear os eventos à medida que acontecem.

Uma ampla lista de Métricas está disponível e é possível agrupá-las por **Catálogo**, **Canal de Importação** e **Modelo de Recomendação**, cada um apresentando suas métricas. Você também pode selecionar múltiplos catálogos para comparação e avaliar seu desempenho.

Estas são todas as métricas disponíveis para o recurso de Catálogos:

* [Contagem de Jobs (Tarefas) de Importação](cs2-metrics.md#contagem-de-jobs-de-importacao)
* [Duração do Job (Tarefa) de Importação](cs2-metrics.md#duracao-do-job-de-importacao)
* [Taxa de Falha do Job (Tarefa) de Importação](cs2-metrics.md#taxa-de-falha-do-job-de-importacao)
* [Problemas no Job (Tarefa) de Importação](cs2-metrics.md#problemas-no-job-de-importacao)
* [Bytes Processados no Job (Tarefa) de Importação](cs2-metrics.md#taxa-de-falha-do-job-de-importacao)
* [Registros Processados no Job (Tarefa) de Importação](cs2-metrics.md#registros-processados-no-job-de-importacao)
* [Contagem de Adições de Produto ao Carrinho](cs2-metrics.md#contagem-de-adicoes-de-produto-ao-carrinho)
* [Contagem de Produtos](cs2-metrics.md#contagem-de-produtos)
* [Contagem de Pedidos de Produto](cs2-metrics.md#contagem-de-pedidos-de-produto)
* [Contagem de Visualizações de Produto](cs2-metrics.md#contagem-de-visualizacoes-de-produto)
* [Produtos Adicionados](cs2-metrics.md#produtos-adicionados)
* [Produtos Removidos](cs2-metrics.md#produtos-removidos)
* [Produtos Atualizados](cs2-metrics.md#produtos-atualizados)
* [Contagem de Recomendações de Produto](cs2-metrics.md#contagem-de-recomendacoes-de-produto)
* [Contagem de Cliques em Recomendação](cs2-metrics.md#contagem-de-cliques-em-recomendacao)
* [Taxa de Preenchimento de Recomendação](cs2-metrics.md#taxa-de-preenchimento-de-recomendacao)
* [Contagem de Requisições de Recomendação](cs2-metrics.md#contagem-de-requisicoes-de-recomendacao)
* [Contagem de Visualizações de Recomendação](cs2-metrics.md#contagem-de-visualizacoes-de-recomendacao)
