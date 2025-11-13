# Faturamento de CS2

A seção de faturamento por serviço de armazenamento de catálogos está disponível na página de faturas. Ela contém informações sobre cada item faturado relacionado ao CS2 e está dividida em 6 subseções.

<figure><img src="../../.gitbook/assets/image (815).png" alt=""><figcaption><p>Seção de Faturamento de CS2</p></figcaption></figure>

{% hint style="info" %}
Na BMS, priorizamos a transparência ao exibir cada detalhe de sua fatura. Visite nossa [Página Inicial de Faturamento](../billing.md) para entender como as faturas são estruturadas.
{% endhint %}

Abaixo está uma explicação de cada uma dessas seções com seus respectivos detalhes.

### Gerenciamento de Catálogos <a href="#catalog-management" id="catalog-management"></a>

Esta subseção descreve os custos associados ao gerenciamento de catálogos. Exclusões são gratuitas, e cada serviço nesta seção inclui uma cota gratuita de 1.000 requisições, exceto pelo armazenamento, que é cobrado com base no número de catálogos armazenados e na duração de seu armazenamento.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 134927.png" alt=""><figcaption><p>Gerenciamento de Catálogos</p></figcaption></figure>

_**Exemplo**: Nesta imagem, foram consumidas quase 1.039 horas-catálogo, o que equivale a 1 catálogo armazenado por um mês junto com outro catálogo armazenado por alguns dias, resultando em uma cobrança de $1,08. Você também pode observar que nenhuma cobrança foi aplicada aos outros serviços consumidos, uma vez que a cota gratuita não foi excedida._

### Gerenciamento de Canais de Importação <a href="#import-channel-management" id="import-channel-management"></a>

Esta subseção descreve os custos associados ao gerenciamento de canais de importação. Os canais de importação configurados são cobrados com base no número de canais configurados e na duração de sua disponibilidade na plataforma. Os _jobs_ (tarefas) de importação são cobrados de acordo com a quantidade de dados que transferiram. Há uma cota gratuita de 100 requisições para o serviço de iniciar tarefa de importação, após a qual as cobranças incorrerão por requisição. Para os outros serviços na seção, há uma cota gratuita de 1.000 requisições, após a qual os serviços serão cobrados por requisição.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 135947.png" alt=""><figcaption><p>Gerenciamento de Canais de Importação</p></figcaption></figure>

_**Exemplo**: Nesta imagem, você notará que para a maioria dos serviços a cota gratuita não foi excedida e, portanto, nenhuma cobrança foi aplicada. Também é possível observar que quase 325 horas-canal foram consumidas, o que equivale a ter 1 canal de importação configurado por quase duas semanas, resultando em uma cobrança de $0,34. Você pode ver que quase 5 GB foram transferidos neste período, resultando em uma fatura de $0,42. Após atingir a cota, o serviço de listagem_ de tarefas de importação foi cobrado por requisição, resultando em uma cobrança de $0,28. Portanto, este cliente será cobrado em $1,03 pelos serviços nesta subseção.

### Modelo de Recomendação <a href="#recommendation-model" id="recommendation-model"></a>

Nesta subseção, você encontrará os detalhes de custo para os modelos de recomendação. Ações de exclusão são gratuitas, e há uma cota gratuita de 1.000 requisições para cada serviço nesta seção, exceto pelos Modelos Configurados, que são cobrados com base no número de modelos de recomendação que você configurou e na duração de sua disponibilidade e uso.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 140608.png" alt=""><figcaption><p>Modelo de Recomendação</p></figcaption></figure>

_**Exemplo**: Você notará que, nesta imagem, a maioria dos serviços consumidos não excedeu a cota gratuita e, portanto, nenhuma cobrança foi aplicada. É possível observar que quase 835 horas-modelo foram consumidas, o que equivale a 1 modelo configurado por quase um mês inteiro, resultando em uma fatura de $0,87._

### Mecanismo de Recomendação <a href="#recommendation-engine" id="recommendation-engine"></a>

Esta subseção detalha os custos relacionados ao uso do mecanismo de recomendação. Há uma cota gratuita de 1.000 requisições; após exceder esta cota, a cobrança é aplicada por requisição de recomendação de produto.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 140715 (1).png" alt=""><figcaption><p>Mecanismo de Recomendação</p></figcaption></figure>

_**Exemplo**: Nesta imagem, a cota gratuita não foi excedida e, portanto, nenhuma cobrança incidirá pelos serviços._

### Gerenciamento de Produtos <a href="#product-management" id="product-management"></a>

Esta subseção contém os detalhes de custo relacionados ao gerenciamento de produtos. Exclusões são gratuitas. Exceto pelo armazenamento, cada serviço nesta seção tem uma cota gratuita de 1.000 requisições, após a qual você será cobrado por requisição. O armazenamento é cobrado com base no número de produtos que você armazenou e na duração de seu armazenamento.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 140958.png" alt=""><figcaption><p>Gerenciamento de Produtos</p></figcaption></figure>

_**Exemplo**: Você observará, nesta imagem, que não houve cobranças para os serviços que não excederam a cota gratuita. Após exceder a cota, os serviços de criação de produtos e de atualização de produtos foram cobrados por requisição. Houve quase 35 mil requisições de criação de produtos, resultando em uma fatura de $0,52, e quase 35 milhões de requisições de atualização de produtos, resultando em uma fatura de $513,17. Você também pode notar que quase 208 milhões de horas-produto foram consumidas, resultando em uma fatura de $28,85, totalizando uma fatura de $542,55 pelos serviços na seção._

### Rastreamento de Catálogo <a href="#catalog-tracking" id="catalog-tracking"></a>

Esta subseção contém os detalhes de custo relacionados ao rastreamento de catálogo. Cada serviço nesta seção tem uma cota gratuita de 1.000 requisições, após a qual você será cobrado por requisição.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-09 142247.png" alt=""><figcaption><p>Rastreamento de Catálogo</p></figcaption></figure>

_**Exemplo**: Nesta imagem, você notará que uma cota gratuita de 1.000 requisições foi dada a cada serviço. Após exceder esta cota, as cobranças foram aplicadas com base no número de requisições usadas. Houve quase 151 mil requisições para rastreamento de eventos de produto, resultando em uma fatura de $1,51, e quase 31 mil requisições de rastreamento de eventos de recomendação, resultando em uma fatura de $0,31, totalizando $1,82 pelos serviços na seção._

{% hint style="info" %}
Todos os produtos geram métricas assim que você começa a usá-los. Essas métricas são cobradas e são cruciais para entender o uso e o desempenho da sua plataforma BMS. A [Aba de Monitoramento](../monitoring/monitoring-billing.md) é responsável por essas métricas e exibirá a cobrança relacionada.

A BMS foca na transparência e mostrará a você os custos de todos os recursos dentro de cada produto.
{% endhint %}
