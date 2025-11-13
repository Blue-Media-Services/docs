# Faturamento de DSP

A seção de faturamento de Campanhas conterá todos os itens faturados relacionados a campanhas e está dividida em 2 subseções.

<figure><img src="../../.gitbook/assets/image (652).png" alt=""><figcaption><p>Seção de Faturamento de DSP</p></figcaption></figure>

{% hint style="info" %}
Na BMS, priorizamos a transparência ao exibir cada detalhe de sua fatura. Visite nossa documentação de [Faturamento](../billing.md) para entender como as faturas são estruturadas.
{% endhint %}

## Como Suas Faturas são Compostas? <a href="#how-is-your-billing-composed" id="how-is-your-billing-composed"></a>

Ao criar e iniciar uma campanha, é necessário usar múltiplos produtos e recursos da nossa plataforma para ter tudo configurado para o início da campanha. Note que os faturamentos da campanha não se baseiam apenas no orçamento diário definido.

### Faturamento vs. Orçamento <a href="#billing-x-budget" id="billing-x-budget"></a>

Nosso faturamento funciona com base no uso de cada produto; é o custo efetivo para cada produto com base no uso, medido por cada requisição enviada a uma API, armazenamento e mídia.

### Armazenamento <a href="#storage" id="storage"></a>

Ao executar uma campanha, múltiplos produtos são usados para construir seus componentes. Como resultado, o armazenamento de cada criativo, grupo de criativos, anúncio e item de mídia incorrerá em cobranças. Nos casos em que a conta acumula muitos desses itens, pode haver um impacto significativo no faturamento mensal. Portanto, realizar limpezas regulares de itens não utilizados é uma boa prática para manter um saldo de cobrança gerenciável.

_**Exemplo:** Mesmo quando uma campanha está inativa, as cobranças ainda podem ser aplicadas porque os criativos e anúncios criados para essa campanha continuam a incorrer em custos de armazenamento._

### Mídia <a href="#media" id="media"></a>

Toda a mídia carregada para a biblioteca incorre em custos de armazenamento e de requisição de download. Cada vez que um usuário final visualiza sua mídia em uma campanha, um custo é gerado tanto para armazenamento quanto para download. Esses custos variam com base no tamanho de cada arquivo de mídia, pois eles consomem espaço de armazenamento nos servidores da BMS. Para ajudar a gerenciar essas despesas, considere usar mídias hospedadas em seus próprios servidores.

_**Exemplo:** Uma mídia com 3MB de tamanho terá um custo diferente de uma mídia com 5MB. Ao hospedar essa mídia em seu próprio servidor, a BMS não cobrará por essa mídia._

### Orçamento Diário <a href="#daily-budget" id="daily-budget"></a>

O orçamento diário definido para uma campanha funciona como um acelerador, ajudando você a controlar o quanto pretende gastar. O valor real gasto ao final do dia pode variar com base nas configurações de público-alvo, nas configurações de lance e na mídia utilizada na campanha.

Ao definir seu orçamento diário, ele é usado em quatro tipos diferentes para entregar uma campanha por completo: **Impressões**, **Entregas**, **Realização de Lances** e **Recomendações**.

#### Orçamento Gasto em Impressões <a href="#budget-spent-on-impressions" id="budget-spent-on-impressions"></a>

Este orçamento é gasto com base nos lances vencidos, sendo o valor pago ao _publisher_ pelo direito de exibir anúncios em seu site. Na fatura, isso é representado como o custo de mídia (a soma de todos os lances vencedores) mais uma taxa de plataforma de 20%.

<figure><img src="../../.gitbook/assets/image (920).png" alt=""><figcaption><p>Métrica de Orçamento Gasto em Impressões</p></figcaption></figure>

_**Exemplo:** Neste caso, o orçamento gasto em impressões foi de mais de $0,50 a um máximo de $0,75. Esta métrica será exibida em Gerenciamento de orçamento e Mídia como o Custo de Mídia. Ao remover a taxa de plataforma de 20%, é possível conciliar os valores._

<figure><img src="../../.gitbook/assets/image (921).png" alt=""><figcaption><p>Faturamento de Orçamento Gasto em Impressões</p></figcaption></figure>

#### Orçamento Gasto em Entregas <a href="#budget-spent-on-deliveries" id="budget-spent-on-deliveries"></a>

Este orçamento refere-se ao custo total de entrega de um anúncio, que inclui as despesas combinadas de Servidor de Anúncios, Monitoramento e Mídia. O custo do servidor de anúncios cobre as requisições de API necessárias para entregar o anúncio, os custos de Monitoramento capturam as métricas e as exibem no painel, e os custos de Mídia cobrem o download da mídia associada. Na fatura, esses custos aparecem em Servidor de Anúncios, Mídia e Monitoramento. Este custo pode variar com base no tamanho da mídia; arquivos de mídia maiores resultarão em despesas maiores.

<figure><img src="../../.gitbook/assets/image (922).png" alt=""><figcaption><p>Métrica de Orçamento Gasto em Entregas</p></figcaption></figure>

_**Exemplo:** Nesta métrica, você pode ver que a cada hora está sendo gasto mais de $0,01 até $0,025 apenas em entregas. Este valor será deduzido do orçamento diário, embora não esteja relacionado ao lance em si._

#### Orçamento Gasto Realizando Lances <a href="#budget-spent-placing-bids" id="budget-spent-placing-bids"></a>

Este custo está associado à despesa operacional de realizar lances. Cada vez que um lance é feito, ele se alinha com os públicos-alvo da campanha, exigindo que o sistema filtre todo o inventário disponível com base nas preferências da campanha para garantir um lance preciso. Este processo incorre em cobranças, embora representem uma pequena porcentagem do orçamento diário total. Em seu extrato de cobrança, a seção de Leilão em Tempo Real (_Real-Time Bidding_) incluirá um item de linha "Lances Realizados", que corresponde às métricas de realização de lances de sua campanha.

<figure><img src="../../.gitbook/assets/image (919).png" alt=""><figcaption><p>Métrica de Orçamento Gasto Realizando Lances</p></figcaption></figure>

_**Exemplo:** Nesta métrica, nota-se que o orçamento gasto com custos operacionais foi de mais de $0,05 a um máximo de $0,13. Este custo será listado em sua cobrança como Leilão em Tempo Real e corresponderá aos custos operacionais de sua campanha._

<figure><img src="../../.gitbook/assets/image (918).png" alt=""><figcaption><p>Cobrança de Realização de Lances</p></figcaption></figure>

#### Orçamento Gasto com Recomendações <a href="#budget-spent-on-recommendations" id="budget-spent-on-recommendations"></a>

Ao usar Banners Dinâmicos, você será cobrado pelo uso da chamada de API para uma recomendação, devido ao custo operacional de vincular seus públicos-alvo a uma recomendação. Se uma campanha não estiver usando Banners Dinâmicos, não haverá custos.

<figure><img src="../../.gitbook/assets/image (880).png" alt=""><figcaption><p>Métrica de Orçamento Gasto com Recomendações</p></figcaption></figure>

_**Exemplo:** Nesta métrica, nota-se que o orçamento gasto foi de mais de $0,05 até $0,08 a cada 12 horas, valor que é deduzido do orçamento diário da campanha._

## Gerenciamento de Orçamento e Mídia <a href="#budget-management-and-media" id="budget-management-and-media"></a>

No gerenciamento de orçamento e mídia, as faturas relacionadas à BMS exibem a disponibilidade de orçamento atual, as requisições geradas quando você altera ou define um orçamento para uma campanha, e o custo de mídia mais uma taxa de 20% da BMS. O custo de mídia é baseado no valor pago a um _publisher_ para exibir seu anúncio.

<figure><img src="../../.gitbook/assets/image (653).png" alt=""><figcaption><p>Itens de Gerenciamento de Orçamento e Mídia</p></figcaption></figure>

_**Exemplo:** Nesta fatura, um custo de mídia de $4.014,89 mais CPM é observado. Este custo é baseado em $3.345,74, que serão repassados aos publishers que exibiram seu anúncio, e um adicional de $669,15 da taxa de 20% pelo uso dos lances da BMS. A disponibilidade de orçamento da campanha também foi cobrada por exceder 1.000.000 de requisições. A um custo de $0,10 por 1.000.000 de requisições, isso totalizou $0,72. Após somar todas as faturas, o custo total atingiu $4.015,61._

## Gerenciamento de Campanhas <a href="#campaign-management" id="campaign-management"></a>

Na fatura de gerenciamento de campanhas, serão exibidos os custos de qualquer ação na página da campanha e do armazenamento da campanha. Cada vez que você cria, habilita ou desabilita campanhas, conta como uma requisição. Se o número de requisições exceder 1.000 durante um mês, haverá um custo. As campanhas são cobradas mesmo que estejam inativas. A BMS conta cada segundo que uma campanha está listada, ativa ou não, e converte segundos em horas, cobrando $0,75 por campanha por mês, com base em um mês de 720 horas.

<figure><img src="../../.gitbook/assets/image (654).png" alt=""><figcaption><p>Itens de Gerenciamento de Campanhas</p></figcaption></figure>

_**Exemplo:** Neste caso, como nenhuma requisição atingiu a marca de 1.000, não haverá cobranças por ações realizadas na página de campanhas. No entanto, como havia campanhas em execução ou listadas, um total de 2.201,09 horas de campanha foram cobradas, o que equivale a cerca de 3 campanhas em execução por um mês inteiro. Isso resultou em um custo total de $2,29. Note que as campanhas são cobradas por estarem listadas, ativas ou não, então excluir uma campanha interromperá cobranças futuras._

{% hint style="info" %}
Todos os produtos geram métricas assim que você começa a usá-los. Essas métricas são cobradas e são cruciais para entender o uso e o desempenho da sua plataforma BMS. A [Aba de Monitoramento](../monitoring/monitoring-billing.md) é responsável por essas métricas e exibirá a cobrança relacionada.\
A BMS é focada na transparência e mostrará os custos de todos os recursos dentro de cada produto.
{% endhint %}
