---
description: Learn more about Blueprints and how to work with them!
---

# Blueprints

_Blueprints_ são modelos para a criação de anúncios de forma rápida e eficiente. Esses modelos pré-fabricados permitem que você codifique banners dinâmicos usando linguagens de desenvolvimento web, criando anúncios mais envolventes e melhorando os resultados esperados.

Construídos com linguagens de web design, os _Blueprints_ oferecem a flexibilidade de criar banners dinâmicos. Mesmo que você não esteja familiarizado com linguagens de desenvolvimento web, pode usar com confiança um dos _Blueprints_ pré-fabricados disponíveis.

## Gerenciando Blueprints <a href="#managing-blueprints" id="managing-blueprints"></a>

<figure><img src="../../../.gitbook/assets/Captura de tela 2024-12-05 072802.png" alt=""><figcaption><p>Lista de Blueprints</p></figcaption></figure>

Você terá alguns modelos de _blueprint_ públicos disponíveis para uso, então mesmo que não esteja familiarizado com linguagens de desenvolvimento web, poderá criar e usar _blueprints_ facilmente. Você também pode criar um _blueprint_ com seus próprios parâmetros, codificando-o; no entanto, esta opção pode exigir habilidades de desenvolvimento web.

### **C**riando um Blueprint <a href="#creating-a-blueprint" id="creating-a-blueprint"></a>

Clique em ![create blueprint](<../../../.gitbook/assets/image (889).png>) para começar a criar seu _blueprint_.

<figure><img src="../../../.gitbook/assets/image (886).png" alt=""><figcaption><p>Criação de Blueprints</p></figcaption></figure>

1. Preencha os Detalhes:
   * Nome: Defina um nome para o seu _blueprint_.
   * Tags: Defina tags para uma melhor organização.
   * Disponibilidade: Selecione se você quer que este _blueprint_ seja público ou privado. _Blueprints_ públicos estarão disponíveis para todos na BMS.
   * Gerar Tamanhos: Selecione em quais tamanhos este _blueprint_ irá construir seus criativos.
   *   Parâmetros: Clique em ![](<../../../.gitbook/assets/image (308).png>) para criar um novo grupo de parâmetros.\


       <figure><img src="../../../.gitbook/assets/image (327).png" alt=""><figcaption><p>Criador de Grupo de Parâmetros</p></figcaption></figure>

       * Nome: Defina um nome para este grupo de parâmetros.
       * Descrição: Defina uma descrição para o grupo de parâmetros.
       * Clique em ![](<../../../.gitbook/assets/image (15).png>) para salvar seu grupo de parâmetros.
2.  Após criar o grupo de parâmetros, você pode começar a codificar seu banner na caixa de código. Em seguida, configure os parâmetros do seu código para alinhá-los com os do grupo de parâmetros. Para adicionar um novo parâmetro ao grupo, clique em <img src="../../../.gitbook/assets/image (310).png" alt="" data-size="line"> e preencha os detalhes:



    <figure><img src="../../../.gitbook/assets/image (335).png" alt=""><figcaption><p>Criador de Parâmetros - Tipos</p></figcaption></figure>

    * ID do Parâmetro: Use este identificador para inserir o valor fornecido pelo usuário em seu template.
    * Nome: Defina um nome para o seu parâmetro.
    * Descrição: Defina uma descrição para o seu parâmetro.
    * Tipo: Selecione o tipo de dados da entrada:
      *   **String**

          <figure><img src="../../../.gitbook/assets/image (328).png" alt=""><figcaption><p>Editor de Parâmetros - String</p></figcaption></figure>

          * Comprimento Mínimo: Defina um comprimento mínimo para a entrada.
          * Comprimento Máximo: Defina um comprimento máximo para a entrada.
          * Regex de Validação: Insira o padrão usado para a validação da string.
          * Mensagem de Validação: Esta mensagem é exibida ao usuário se o padrão de validação não corresponder.
          * Selecione entre as opções:
            * Linha Única: Cria um campo para inserir uma única linha de texto.
            * Múltiplas Linhas: Cria um campo que permite inserir várias linhas de texto.
            * Valor Inicial: Este é o valor inicial que o sistema usará ao criar um novo _build_.
      *   Booleano



          <figure><img src="../../../.gitbook/assets/image (333).png" alt=""><figcaption><p>Editor de Parâmetros - Booleano</p></figcaption></figure>

          * Valor Inicial: Marque a caixa se o valor inicial for verdadeiro, desmarque se for falso.
      *   Escolha



          <figure><img src="../../../.gitbook/assets/image (334).png" alt=""><figcaption><p>Editor de Parâmetros - Escolha</p></figcaption></figure>

          * Rótulo: Insira o rótulo do seu parâmetro.
          * Valor: Insira o valor associado ao rótulo.
          * Adicione quantos rótulos precisar clicando em ![Add](<../../../.gitbook/assets/image (891).png>).
          * Valor Inicial: Escolha um dos rótulos configurados como o valor inicial.
      *   **Código**



          <figure><img src="../../../.gitbook/assets/image (336).png" alt=""><figcaption><p>Editor de Parâmetros - Código</p></figcaption></figure>

          * Tipo: Selecione a linguagem de programação
          * Caixa de Código: Insira seu código na caixa de código.
      *   **Cor**



          <figure><img src="../../../.gitbook/assets/image (330).png" alt=""><figcaption><p>Editor de Parâmetros - Cor</p></figcaption></figure>

          * Valor Inicial: Insira o código de cor hexadecimal, ou clique na caixa de cor para escolher uma cor.
      *   **Número**

          <figure><img src="../../../.gitbook/assets/image (332).png" alt=""><figcaption><p>Editor de Parâmetros - Número</p></figcaption></figure>

          * Mínimo: Insira o valor mínimo a ser aceito.
          * Máximo: Insira o valor máximo a ser aceito.
          * Valor Inicial: Insira o valor inicial do parâmetro.
      *   **ID de Recurso**



          <figure><img src="../../../.gitbook/assets/image (331).png" alt=""><figcaption><p>Editor de Parâmetros - ID de Recurso</p></figcaption></figure>

          * Tipo de Recurso: Escolha entre um catálogo CS2 ou um Modelo de Recomendação CS2 para usar um deles como recurso para seu banner.
          * Valor Inicial: Selecione o catálogo ou modelo de recomendação específico que você deseja usar para este parâmetro.
      *   **URL**



          <figure><img src="../../../.gitbook/assets/image (329).png" alt=""><figcaption><p>Editor de Parâmetros - URL</p></figcaption></figure>

          * Usar seletor de imagens: Marque esta caixa para habilitar o seletor de imagens, no qual você pode escolher imagens de seus criativos já carregados, carregar uma nova se necessário, ou informar a URL da imagem.
          * Valor Inicial: Insira o valor inicial para a URL da imagem.
    * Clique em ![save](<../../../.gitbook/assets/image (892).png>) para salvar seu parâmetro.
3. Continue adicionando grupos de parâmetros e parâmetros até que as necessidades do seu negócio sejam satisfeitas.&#x20;
4. Use os parâmetros de sistema disponíveis para personalizar seu template:
   * ID da Conta: Esta opção insere em seu template o ID da conta onde o _build_ é criado.
   * Largura do Banner: Insere a largura na qual o banner será renderizado.
   * Altura do Banner: Insere a altura na qual o banner será renderizado.
5. Use as macros disponíveis com suas URLs, algumas delas são:
   * URL de Clique Sem Escape: Esta macro será substituída pela URL do rastreador de cliques sem escape da BMS. Use esta opção quando a BMS for o primeiro rastreador de cliques na cadeia.
   * URL de Clique Com Escape: Esta macro será substituída pela URL do rastreador de cliques com escape da BMS. Use esta opção quando a BMS for o segundo rastreador de cliques na cadeia.
   * URL de Clique com Escape Duplo: Esta macro será substituída pela URL do rastreador de cliques com escape duplo da BMS. Use esta opção quando a BMS for o terceiro rastreador de cliques na cadeia.
   * Cache Buster: Esta macro será substituída por um número aleatório que pode ser usado para evitar o cache.
   * Contexto do Anúncio com Escape: Esta macro será substituída por um objeto JSON com escape contendo dados sobre o contexto do anúncio, como o ID da campanha e dados do usuário.
6. Após finalizar todas as configurações do seu _blueprint_, clique em <img src="../../../.gitbook/assets/image (309).png" alt="" data-size="line"> para salvar seu _blueprint_.

### Usando um Blueprint Existente <a href="#using-an-existing-blueprint" id="using-an-existing-blueprint"></a>

Também é possível usar um _blueprint_ existente. Você pode duplicar um _blueprint_ que já possui para reutilizar alguns de seus parâmetros clicando em <img src="../../../.gitbook/assets/image (21).png" alt="" data-size="line"> na mesma linha do _blueprint_ que deseja duplicar. Além disso, você pode usar um _blueprint_ público. Desligue a opção <img src="../../../.gitbook/assets/image (22).png" alt="" data-size="line"> "próprios", acima da lista de _blueprints_, escolha um dos _blueprints_ disponíveis e clique em <img src="../../../.gitbook/assets/image (23).png" alt="" data-size="line"> na mesma linha do _blueprint_ público que deseja usar. Ligue novamente a opção <img src="../../../.gitbook/assets/image (24).png" alt="" data-size="line"> "próprios" e, em seguida, clique em <img src="../../../.gitbook/assets/image (25).png" alt="" data-size="line"> para editar o _blueprint_ de acordo com as necessidades do seu negócio.

### Excluindo Blueprints <a href="#deleting-blueprints" id="deleting-blueprints"></a>

Você pode excluir ou arquivar _blueprints_ de acordo com suas necessidades. Para arquivar _blueprints_, clique em <img src="../../../.gitbook/assets/image (26).png" alt="" data-size="line"> na mesma linha do _blueprint_ que deseja arquivar. Para visualizar seus _blueprints_ arquivados, ative a opção <img src="../../../.gitbook/assets/image (27).png" alt="" data-size="line"> "arquivados" acima da lista de _blueprints_.

{% hint style="danger" %}
Atenção! Tenha cuidado ao excluir _blueprints_. Esta ação não pode ser desfeita, e os _builds_ que dependem do _blueprint_ excluído deixarão de funcionar. Todos os dados relacionados, incluindo métricas coletadas anteriormente, também serão excluídos.
{% endhint %}

Para excluir _blueprints_, clique em <img src="../../../.gitbook/assets/image (28).png" alt="" data-size="line"> na mesma linha do _blueprint_ que precisa excluir e, em seguida, confirme a ação clicando em <img src="../../../.gitbook/assets/image (29).png" alt="" data-size="line">.
