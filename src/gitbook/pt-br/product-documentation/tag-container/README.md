# Contêineres de Tags

Esse recurso permite criar um contêiner de tags personalizado para instalar várias tags e scripts a partir de um único trecho de código.

<figure><img src="../../.gitbook/assets/image (537).png" alt=""><figcaption><p>Lista de Contêineres de Tags</p></figcaption></figure>

### Criando Contêineres de Tags <a href="#creating-tag-containers" id="creating-tag-containers"></a>

Siga os passos abaixo para criar seu Contêiner de Tags. Este processo irá guiá-lo pelos passos necessários para configurar um contêiner personalizado que pode armazenar várias tags e scripts, simplificando o gerenciamento e a implementação dos códigos de rastreamento em seu site.

{% hint style="info" %}
Usamos cookie pools e rastreadores como exemplos de scripts para explicar esse recurso, mas você pode usar qualquer script ou tag que precisar.
{% endhint %}

1.  Clique em <img src="../../.gitbook/assets/image (523).png" alt="" data-size="line"> para começar a criar seu Contêiner de Tags.<br>

    <figure><img src="../../.gitbook/assets/Captura de tela 2024-10-01 114707.png" alt=""><figcaption><p>Editor de Contêiner de Tags</p></figcaption></figure>
2. Preencha os detalhes:
   * Nome: Defina um nome para seu contêiner de tags.
   * Tags: Defina tags para melhor organização.
   * _Template_: Cole os scripts e tags que você precisa incluir no seu contêiner de tags. No exemplo mostrado, foi usado um script de Cookie Pools da BMS. Note que os valores do ID da conta ("acc") e do ID do Cookie Pool ("cpid") foram substituídos pelos espaços reservados "\{{acc\}}" e "\{{cpid\}}". Isso permite que o contêiner de tags seja usado de forma dinâmica. Da mesma forma, um script de rastreadores da BMS também foi adicionado.
   * Parâmetros Disponíveis: Os parâmetros aparecerão nesta seção com base na sua Entrada de Exemplo (_Sample Input_). Você pode clicar neles para copiar suas referências.
   * Entrada de Exemplo: Aqui você fornecerá um exemplo de entrada para seu contêiner de tags. No exemplo mostrado, há quatro parâmetros configurados no exemplo de entrada:
     * "e": Refere-se ao evento que deve ser rastreado usando nosso script de rastreadores.
     * "t": Refere-se ao ID do rastreador a ser usado.
     * "acc": Refere-se ao ID da conta BMS.
     * "cpid": Refere-se ao ID do cookie pool.
   * Visualização: Esta seção mostra como seu contêiner de tags ficará depois que você preencher os parâmetros.
3. Após terminar suas edições, clique em <img src="../../.gitbook/assets/image (524).png" alt="" data-size="line"> para salvar seu contêiner de tags.

### Instalando seu Contêiner de Tags <a href="#installing-your-tag-container" id="installing-your-tag-container"></a>

Siga os passos na aba de instruções de instalação para instalar corretamente seu contêiner de tags.

<figure><img src="../../.gitbook/assets/image (525).png" alt=""><figcaption><p>Instruções de Instalação</p></figcaption></figure>

1. Copie o script usando o botão de copiar <img src="../../.gitbook/assets/image (526).png" alt="" data-size="line">.
2. Substitua os parâmetros pelos valores correspondentes.
3. Cole-o no código do seu site.

### Editando ou Excluindo Contêineres de Tags <a href="#editing-or-deleting-tag-containers" id="editing-or-deleting-tag-containers"></a>

Todos os campos no editor de contêiner de tags estão disponíveis para edição. Clique em <img src="../../.gitbook/assets/image (527).png" alt="" data-size="line"> para editar seu contêiner de tags.

{% hint style="danger" %}
_Atenção! Tenha cuidado ao excluir contêineres de tags, pois essa ação não pode ser desfeita e todos os dados relacionados, incluindo métricas coletadas anteriormente, também serão excluídos._
{% endhint %}

É possível excluir contêineres de tags clicando em <img src="../../.gitbook/assets/image (528).png" alt="" data-size="line"> na mesma linha do contêiner que você deseja excluir, e depois clicando em <img src="../../.gitbook/assets/image (529).png" alt="" data-size="line"> para confirmar essa ação.

Como alternativa, você pode arquivar contêineres de tags para ajudar na organização. Isso pode ser feito clicando em <img src="../../.gitbook/assets/image (530).png" alt="" data-size="line"> na mesma linha do contêiner que você deseja arquivar. Para visualizar os contêineres de tags arquivados, ative o interruptor 'Arquivado' ![](<../../.gitbook/assets/image (531).png>), localizado logo acima da lista de contêineres. Para desarquivar um contêiner de tags, clique em <img src="../../.gitbook/assets/image (532).png" alt="" data-size="line"> na mesma linha do contêiner que deseja desarquivar.

### Aba de Métricas <a href="#metrics-tab" id="metrics-tab"></a>

Após concluir a instalação dos seus Contêineres de Tags e usá-los efetivamente, eles começarão a preencher as métricas apresentadas. Abaixo, você encontra todas as métricas relacionadas aos Contêineres de Tags.

* [Taxa de Falhas](tag-container-metrics.md#taxa-de-falhas)
* [Contagem de Requisições](tag-container-metrics.md#contagem-de-requisicoes)
