# Métricas de DMP

Estas são todas as métricas disponíveis no produto DMP para analisar o desempenho de seus _cookie pools_ e rastreadores. Além disso, ao revisar as métricas, você sempre pode usar o <img src="../../.gitbook/assets/image (1089).png" alt="" data-size="line"> para acessar nossos artigos sobre uma métrica específica.

{% hint style="info" %}
Você pode aprender mais sobre como as métricas são tratadas visitando a página de [Métricas](../metrics.md).
{% endhint %}

### Contagem de Expirações <a href="#expiration-count" id="expiration-count"></a>

Esta métrica exibe quantos cookies expiraram dentro do período de tempo configurado. Os cookies expiram com base no TTL, que é o número de dias após o qual um cookie expirará, configurado ao criar o cookie pool.

<figure><img src="../../.gitbook/assets/image (1090).png" alt=""><figcaption><p>Contagem de Expirações</p></figcaption></figure>

_**Exemplo**: Você cria um cookie pool com um TTL de sete dias e o instala em sua página inicial. Os cookies gerados pelo acesso dos seus usuários estarão disponíveis para segmentação de públicos-alvo por sete dias. Após esse período, os cookies expirarão. Isso significa que em uma campanha de retargeting, por exemplo, você impactará usuários que visitaram seu site nos últimos sete dias. Neste gráfico, você pode observar que em 19 de junho, pouco menos de 5 cookies expiraram, em 20 de junho nenhum cookie expirou, e em 21 de junho pouco menos de 5 cookies expiraram, e assim por diante._

### Tamanho Máximo de Cookie Pool <a href="#max-size" id="max-size"></a>

Esta métrica mostra a quantidade máxima de cookies permitida no _pool_, conforme configurado.

<figure><img src="../../.gitbook/assets/image (1091).png" alt=""><figcaption><p>Tamanho Máximo</p></figcaption></figure>

_**Exemplo**: Ao criar ou editar um cookie pool, você pode definir a quantidade máxima de cookies no pool. Isso limitará o número total de cookies que seu pool pode conter. Neste gráfico, você pode observar que um tamanho máximo de 100.000 cookies foi definido para este cookie pool._

### Tamanho de Cookie Pool <a href="#size" id="size"></a>

Esta métrica mostra o tamanho real do pool, ou seja, ela mostrará quantos cookies estão ou estiveram no pool dentro do período de tempo configurado.

<figure><img src="../../.gitbook/assets/image (1092).png" alt=""><figcaption><p>Tamanho</p></figcaption></figure>

_**Exemplo**: Neste gráfico, você pode observar o tamanho de um cookie pool no período de tempo definido. Esta métrica pode ser usada para obter conhecimento sobre quantos cookies são gerados dentro do período configurado, o que permitirá que você defina um tamanho máximo para o pool que esteja na mesma faixa do número de usuários em seu site._

### Contagem de Sincronizações <a href="#sync-count" id="sync-count"></a>

Esta métrica mostra o número de sincronizações de cookies, ou seja, mostra quando um cookie coletado foi sincronizado com nossa plataforma e, posteriormente, também com as exchanges, o que permite segmentar usuários com mais precisão.

<figure><img src="../../.gitbook/assets/image (1093).png" alt=""><figcaption><p>Contagem de Sincronizações</p></figcaption></figure>

_**Exemplo**: Neste gráfico, você pode observar o número de sincronizações que ocorreram em um período de tempo definido. Quando um usuário acessa seu site, um cookie será solicitado para ele. Após receber este cookie, será analisado se este usuário já possui um cookie ou não. Se possuir, o novo cookie será sincronizado com o já existente, atualizando seus dados na plataforma. Se não possuir, um cookie será criado para ele na plataforma._

### Tempo Até a Expiração <a href="#time-until-expiration" id="time-until-expiration"></a>

Esta métrica mostra a mediana do tempo restante que um cookie ainda está disponível no pool até expirar no período de tempo determinado.

<figure><img src="../../.gitbook/assets/image (1094).png" alt=""><figcaption><p>Tempo Até a Expiração</p></figcaption></figure>

_**Exemplo**: Ao criar seu cookie pool, você pode definir o número de dias em que um cookie irá expirar. Esta métrica mostra quanto tempo você tem até a expiração de um cookie. Neste gráfico, o período de tempo foi de 1 semana, dividido em períodos diários, representados como pontos. Você pode observar que em 20 de junho havia menos de 1 dia até que alguns dos cookies no pool expirassem._

### Contagem de Execução de Ação <a href="#action-execution-count" id="action-execution-count"></a>

Esta métrica mostra quantas ações foram executadas pelo seu rastreador no período de tempo configurado. Você também pode agrupar os dados fornecidos por rastreador ou por evento, de acordo com suas necessidades.

<figure><img src="../../.gitbook/assets/image (1095).png" alt=""><figcaption><p>Contagem de Execução de Ação</p></figcaption></figure>

_**Exemplo**: Neste gráfico, você pode observar um aumento no número de ações às 6h da manhã. O gráfico exibe um período de 3 horas, dividido em intervalos de 5 minutos, representados como pontos de dados. Após criar um rastreador, você precisará configurar eventos e ações. Cada vez que um evento rastreado ocorre, as ações configuradas associadas a esse evento também serão executadas. Por exemplo, um evento de 'adicionar ao carrinho' pode acionar uma ação para rastrear o produto adicionado no catálogo. Esta métrica indica quando e com que frequência a ação é executada dentro desse período._

### Taxa de Falha de Ação <a href="#action-failure-rate" id="action-failure-rate"></a>

Esta métrica mostra quando um evento foi rastreado, mas a ação vinculada a ele falhou. Você também pode agrupar os dados fornecidos por rastreador ou por evento, de acordo com suas necessidades.

<figure><img src="../../.gitbook/assets/image (1096).png" alt=""><figcaption><p>Taxa de Falha de Ação</p></figcaption></figure>

_**Exemplo**: Quando um usuário adiciona um produto ao carrinho em seu site e este evento está configurado para ser rastreado, com uma ação para rastreá-lo no catálogo, o evento em si é rastreado com sucesso. No entanto, a ação para atualizar o catálogo falhou, resultando no não rastreamento do produto. No gráfico, você pode observar que a taxa de falha de ação é tipicamente de 0%. No entanto, há momentos em que a taxa de falha de ação atinge picos próximos a 40%. O gráfico cobre um período de 3 horas, dividido em intervalos de 5 minutos._

### Contagem de Expirações <a href="#expiration-count" id="expiration-count"></a>

Esta métrica mostra a quantidade de expirações de usuários que ocorreram no período de tempo definido.

<figure><img src="../../.gitbook/assets/image (1097).png" alt=""><figcaption><p>Contagem de Expirações</p></figcaption></figure>

_**Exemplo**: Ao configurar um rastreador, você pode definir um período de rastreamento após o qual o usuário expirará. Esta métrica mostra o número de expirações que ocorreram. Neste gráfico, você pode observar que entre 4h e 5h da manhã, quase 50 usuários rastreados expiraram._

### Máximo de Usuários <a href="#maximum-users" id="maximum-users"></a>

Esta métrica mostra o número máximo configurado de usuários a serem adicionados ao rastreador.

<figure><img src="../../.gitbook/assets/image (1098).png" alt=""><figcaption><p>Máximo de Usuários</p></figcaption></figure>

_**Exemplo**: Ao criar ou editar um rastreador, você definirá o número máximo de usuários permitidos a serem adicionados ao seu rastreador. Esta métrica exibe esses dados. Neste gráfico, você pode observar que o rastreador foi configurado para aceitar até 1 milhão de usuários._

### Contagem de Atividades <a href="#activity-count" id="activity-count"></a>

Sempre que um usuário realiza uma atividade rastreada em seu site, ela será rastreada. Esta métrica mostra o número de novas atividades rastreadas dentro de um período de tempo definido. Você também pode agrupar os dados fornecidos por rastreador ou por evento, de acordo com suas necessidades.

<figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption><p>Contagem de Atividades</p></figcaption></figure>

_**Exemplo**: Você tem um evento de 'adicionar ao carrinho' configurado em seu rastreador. Sempre que um usuário adiciona um produto ao carrinho, isso conta como uma atividade. Neste gráfico, você notará que o número de atividades aumenta após as 6h da manhã. Você também observará que este gráfico cobre um período de 3 horas, dividido em intervalos de 5 minutos representados como pontos de dados._

### Valor da Atividade <a href="#activity-value" id="activity-value"></a>

Algumas atividades rastreadas, como adicionar produtos ao carrinho ou comprar um produto, podem ter um valor associado a elas. Esta métrica representa o valor total das atividades rastreadas em seu site dentro de um período de tempo definido.

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption><p>Valor da Atividade</p></figcaption></figure>

_**Exemplo**: Você tem um evento de 'compra' configurado em seu rastreador. Sempre que um usuário conclui uma compra, esta métrica será preenchida com o valor monetário dessa compra. O período de tempo definido para este gráfico foi de 3 dias, dividido em períodos diários. No primeiro período, o valor total dos eventos de compra para este rastreador foi de quase $1.400,00, e nos dias seguintes, esse valor diminuiu para quase $300,00._

### Tempo Até a Expiração <a href="#time-until-expiration" id="time-until-expiration"></a>

Esta métrica mostra o tempo restante que um usuário ainda está disponível no rastreador até expirar no período de tempo determinado.

<figure><img src="../../.gitbook/assets/image (1100).png" alt=""><figcaption><p>Tempo Até a Expiração</p></figcaption></figure>

_**Exemplo**: Ao criar seu rastreador, você pode definir o número de dias em que a atividade rastreada expirará. Esta métrica mostra quanto tempo você tem até a expiração de um usuário. Neste gráfico, o período foi de 1 semana, dividido em períodos diários. Você pode observar que em 20 de junho havia menos de 1 dia até que alguns dos usuários no rastreador expirassem._

### Contagem de Usuários do Rastreador <a href="#tracker-user-count" id="tracker-user-count"></a>

Esta métrica mostrará quantos usuários estavam no rastreador no período de tempo definido.

<figure><img src="../../.gitbook/assets/image (1101).png" alt=""><figcaption><p>Contagem de Usuários do Rastreador</p></figcaption></figure>

_**Exemplo**: Após configurar um rastreador em seu site, os usuários do seu site começarão a ser rastreados. O número de usuários rastreados dentro de um período de tempo definido é o dado mostrado nesta métrica. Neste gráfico, você notará que o número de usuários rastreados entre 4h e 6h da manhã foi de quase 400 mil._

### Contagem de Identificadores Adicionados <a href="#identifiers-added-count" id="identifiers-added-count"></a>

Esta métrica exibe o número total de identificadores adicionados ao _pool_, no período de tempo definido.

<figure><img src="../../.gitbook/assets/image (1136).png" alt=""><figcaption><p>Contagem de Identificadores Adicionados</p></figcaption></figure>

_**Exemplo**: À medida que os usuários de dispositivos móveis navegam pelas páginas do seu site ou aplicativos nos quais você instalou um rastreador configurado para adicionar usuários a um identifier pool, eles serão adicionados ao pool. Neste gráfico, você pode acompanhar o crescimento do seu identifier pool à medida que os identificadores dos usuários são adicionados a ele. O período definido foi de 1 semana, dividido em períodos diários. Você notará que em 31 de dezembro, um pouco mais de 20 identificadores foram adicionados, e nos dias seguintes esse número diminui para 3 por dia, e depois aumenta novamente para 5 em 3 de janeiro._

### Contagem de Identificadores Habilitados <a href="#identifiers-enabled-count" id="identifiers-enabled-count"></a>

Esta métrica mostra o número de identificadores habilitados em pelo menos uma _exchange_, no período de tempo definido.

<figure><img src="../../.gitbook/assets/image (1137).png" alt=""><figcaption><p>Contagem de Identificadores Habilitados</p></figcaption></figure>

_**Exemplo**: À medida que os identificadores são adicionados ao seu pool, a plataforma enviará os identificadores para as ad exchanges selecionadas e verificará se os identificadores estão habilitados em seus bancos de dados. Este processo de sincronização pode ser valioso para campanhas de retargeting._

### Contagem de Identificadores Expirados <a href="#identifiers-expired-count" id="identifiers-expired-count"></a>

Esta métrica exibe o número de Identificadores no pool que expiraram no período de tempo definido.

<figure><img src="../../.gitbook/assets/image (1138).png" alt=""><figcaption><p>Contagem de Identificadores Expirados</p></figcaption></figure>

_**Exemplo**: Você cria um identifier pool com um TTL de sete dias e o instala em seu aplicativo. Os identificadores coletados estarão disponíveis para segmentação por sete dias. Após esse período, os identificadores expirarão. Isso significa que em uma campanha de retargeting, por exemplo, você impactará usuários que usaram seu aplicativo nos últimos sete dias. Neste gráfico, o período definido foi de 1 semana, dividido em períodos diários. Você notará que de 30 de dezembro a 1 de janeiro, houve 1 expiração por dia, depois nenhuma em 2 de janeiro, e depois volta para 1 expiração por dia até 5 de janeiro._

### Contagem de Identificadores Removidos Manualmente <a href="#identifiers-manually-removed-count" id="identifiers-manually-removed-count"></a>

Esta métrica mostra o número de identificadores removidos manualmente do pool, no período de tempo definido.

<figure><img src="../../.gitbook/assets/image (1139).png" alt=""><figcaption><p>Contagem de Identificadores Removidos Manualmente</p></figcaption></figure>

_**Exemplo**: Ao configurar um rastreador para um identifier pool, você poderá selecionar entre adicionar ou remover identificadores do seu pool. Esta métrica exibe a quantidade de identificadores que estão sendo removidos do pool por este processo._

### Tamanho Máximo de Identifier Pool <a href="#max-size" id="max-size"></a>

Esta métrica mostra o número máximo de usuários que o Identifier Pool foi configurado para aceitar, no período de tempo definido.

<figure><img src="../../.gitbook/assets/image (1140).png" alt=""><figcaption><p>Tamanho Máximo</p></figcaption></figure>

_**Exemplo**: Ao criar ou editar um identifier pool, você pode definir o número máximo de identificadores que ele pode conter. Isso limitará o número total de identificadores que seu pool pode conter. Neste gráfico, o período configurado foi de uma semana, dividido em períodos diários. Você notará que o tamanho máximo configurado para este pool não mudou._

### Tamanho de Identifier Pool <a href="#size" id="size"></a>

Esta métrica mostra o tamanho real do _pool_, ou seja, mostrará o número de identificadores que estão ou estiveram no _pool_ dentro do período de tempo configurado.

<figure><img src="../../.gitbook/assets/image (1141).png" alt=""><figcaption><p>Tamanho</p></figcaption></figure>

_**Exemplo**: Neste gráfico, você pode observar o tamanho de um identifier pool no período de tempo definido. Esta métrica pode ser usada para obter conhecimento sobre quantos identificadores são adicionados ao seu pool dentro do período configurado, o que permitirá que você defina um tamanho máximo para o pool que esteja na mesma faixa do número de usuários em seu site. Nesta imagem, você notará que em 30 de dezembro, havia 12 usuários neste pool, e nos dias seguintes este número diminuiu para 10 usuários, e em 5 de janeiro, havia 8 usuários no pool._

### Tempo até a Expiração de Identifier Pool <a href="#time-until-expiration" id="time-until-expiration"></a>

Esta métrica mostra a mediana do tempo restante que um identificador ainda está disponível no _pool_ até expirar no período de tempo determinado.

<figure><img src="../../.gitbook/assets/image (1142).png" alt=""><figcaption><p>Tempo até a Expiração</p></figcaption></figure>

_**Exemplo**: Ao criar seu identifier pool, você pode definir o número de dias em que um identificador adicionado ao pool expirará. Esta métrica mostra a mediana do tempo que você tem até a expiração de um identificador. Neste gráfico, o período definido foi de 1 semana, dividido em períodos diários. Você notará que em 30 de dezembro a mediana era de cerca de 16 dias até a expiração dos identificadores, e nos dias seguintes essa mediana continuou aumentando até 5 de janeiro, quando era de cerca de 23 dias até a expiração._
