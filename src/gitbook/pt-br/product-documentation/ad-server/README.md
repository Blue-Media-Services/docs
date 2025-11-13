# Ad Server

## Produtos <a href="#concepts" id="concepts"></a>

### Criativos <a href="#creatives" id="creatives"></a>

São os menores componentes de nosso ad server. Um criativo representa o código que será entregue ao usuário final quando seu anúncio for exibido.

Você pode fornecer o código HTML diretamente ou a plataforma pode gerar o código HTML para você caso forneça uma imagem e URL de destino.

Os criativos podem estar em um de três estados: rascunho, em revisão e aprovado. Qualquer modificação no conteúdo de um criativo o colocará como rascunho, e ele não será veiculado aos usuários. Você pode enviar quaisquer alterações para revisão e, se tudo estiver de acordo com nossas políticas, o criativo será aprovado.

### Grupos de Criativos <a href="#creative-groups" id="creative-groups"></a>

Os grupos de criativos, como o nome sugere, permitem agrupar vários criativos aplicando pesos diferentes a cada um.

Isso é mais útil ao executar testes A/B com qualquer número de criativos para medir qual deles tem melhor desempenho.

### Anúncios <a href="#a-ds" id="a-ds"></a>

Anúncios são o que o navegador do usuário final solicita do nosso Ad Server. Eles são compostos por uma ou mais regras, em que cada regra específica um conjunto de condições que, uma vez atendidas, direcionarão o usuário para um grupo de criativos específico.

Quando o navegador do usuário final faz a solicitação de anúncio, o grupo de criativos associado à primeira regra que corresponder será entregue. Neste momento, um dos criativos configurados no grupo será selecionado aleatoriamente por peso e então entregue.

### Construtor de Criativos <a href="#creative-builder" id="creative-builder"></a>

Para simplificar a criação de criativos padronizados, você pode usar _Blueprints_ e _Builds_. Esses recursos também podem ser usados para gerar banners dinâmicos contendo seus produtos.

#### Blueprints

_Blueprints_ definem um código HTML base que pode ser gerado dinamicamente com base na entrada do usuário. Os parâmetros necessários para a geração também podem ser personalizados.

#### Builds

Quando você tem um _blueprint_ pronto e deseja criar criativos a partir dele, você cria um _build_. Um _build_ registrará quais tamanhos de criativo você deseja, o _blueprint_ utilizado e todos os parâmetros. Uma vez criado, o _build_ gerará todos os criativos para você. Você pode, a qualquer momento, alterar qualquer parâmetro e os criativos serão atualizados para refletir a mudança.
