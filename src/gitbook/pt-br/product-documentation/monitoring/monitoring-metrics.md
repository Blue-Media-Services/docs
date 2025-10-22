# Métricas de Monitoramento

Estas são todas as métricas disponíveis no recurso de Monitoramento para analisar os dados fornecidos por seus eventos configurados. A aba de métricas de Event Stores apresentará eventos relacionados a todos os _pipes_ de eventos que ocorreram e estarão disponíveis para download. A aba de Pipes de Eventos apresentará métricas relacionadas a todos os seus _pipes_ criados, informando se os _pipes_ estão funcionando corretamente.

{% hint style="info" %}
_Você pode aprender mais sobre como as métricas são tratadas visitando a_ [_página de Métricas_](../metrics.md)_._
{% endhint %}

### Bytes do Fluxo <a href="#stream-bytes" id="stream-bytes"></a>

É preenchida quando há Fluxos de Eventos disponíveis para download. De acordo com o tamanho de cada fluxo de eventos, esta métrica apresentará a soma de todos os bytes dos seus fluxos de eventos.

<figure><img src="../../.gitbook/assets/Stream Bytes.png" alt=""><figcaption><p>Métrica de Bytes do Fluxo</p></figcaption></figure>

_**Exemplo**_: _Após ter um event store populado, ele apresentará fluxos de eventos relacionados aos pipes selecionados. Então, você poderá verificar o tamanho e a data de cada pipe separadamente. O gráfico será preenchido à medida que o tamanho do fluxo aumenta. É possível ver neste gráfico que ele atingiu quase 2 MB de tamanho em uma semana._

### Contagem de Fluxos <a href="#stream-count" id="stream-count"></a>

Apresenta a contagem de cada fluxo de eventos presente em seu _event store_. Se o _event store_ tiver muitos _pipes_ relacionados a ele, a contagem será alta.

<figure><img src="../../.gitbook/assets/Stream Count.png" alt=""><figcaption><p>Métrica de Contagem de Fluxos</p></figcaption></figure>

_**Exemplo:** Ao criar pipes de eventos, você deve selecionar um event store ou um webhook para enviar os dados. Uma vez que você seleciona um event store, cada pipe que você cria para o mesmo event store gerará um fluxo de eventos ao receber dados. É importante notar que, se você tiver muitos pipes de eventos para o mesmo event store, é aconselhável separá-los para organizar melhor seus fluxos de eventos. Neste gráfico, você pode ver que a contagem de fluxos atingiu um pico de quase 200 fluxos._

### Bytes de Upload do Fluxo <a href="#stream-upload-bytes" id="stream-upload-bytes"></a>

Apresenta a quantidade total de bytes carregados para a sua aba de fluxos de eventos, deixando os fluxos disponíveis para download.

<figure><img src="../../.gitbook/assets/Stream Upload Bytes.png" alt=""><figcaption><p>Métrica de Bytes de Upload do Fluxo</p></figcaption></figure>

_**Exemplo:** Cada fluxo de eventos é carregado para o seu event store selecionado após alguns minutos, ficando disponível para download como um arquivo .JSON. A métrica apresentará a soma de todos os bytes dos fluxos de eventos carregados para o seu event store. Neste gráfico, podemos ver que em datas específicas, os dados foram significativamente reduzidos devido à data de expiração de cada fluxo de eventos ou exclusão._

### Contagem de Uploads do Fluxo <a href="#stream-upload-count" id="stream-upload-count"></a>

Esta métrica apresenta a contagem total de uploads, relacionada a cada dado de fluxo de eventos coletado e apresentado para download. Uma vez que eles expirem ou sejam excluídos, a contagem diminuirá.

<figure><img src="../../.gitbook/assets/stream upload count.png" alt=""><figcaption><p>Métrica de Contagem de Uploads do Fluxo</p></figcaption></figure>

_**Exemplo:**_ Neste gráfico, é possível ver que em algumas datas a contagem chegou a quase zero por não haver _pipes_ de eventos ativos ou por causa de uma limpeza. É importante verificar sua contagem de uploads, pois ela pode impactar como você está organizando seus fluxos de eventos. Ter muitos fluxos de eventos para organizar pode ser confuso, então uma limpeza ou otimização deve ser feita de tempos em tempos.

### Bytes de Download do Fluxo <a href="#stream-download-bytes" id="stream-download-bytes"></a>

Esta métrica representa a soma de todos os bytes baixados de seus fluxos de eventos e será preenchida apenas quando o fluxo de eventos for baixado.

<figure><img src="../../.gitbook/assets/Stream Download Bytes.png" alt=""><figcaption><p>Métrica de Bytes de Download do Fluxo</p></figcaption></figure>

_**Exemplo:** Assim que você começar a baixar os dados de seus fluxos de eventos, será informado do número total de bytes baixados a cada dia. Isso ajuda a acompanhar quantos dados foram baixados. Se o volume de dados for alto, indica que muitos eventos foram capturados do fluxo de eventos. Neste gráfico, você pode ver que apenas 2 KB de dados foram baixados._

### Contagem de Downloads do Fluxo <a href="#stream-download-count" id="stream-download-count"></a>

Esta métrica representa os fluxos de eventos baixados, e será preenchida toda vez que você baixar um fluxo de eventos.

<figure><img src="../../.gitbook/assets/Stream Download Count.png" alt=""><figcaption><p>Métrica de Contagem de Downloads do Fluxo</p></figcaption></figure>

_**Exemplo:** Se você se organizar para baixar os dados dos pipes de eventos coletados toda semana ou a cada duas semanas, a métrica o informará para que você não perca o controle de sua programação estabelecida. Neste gráfico, você pode ver que os fluxos de eventos foram baixados apenas após uma semana._

### Bytes Excluídos do Fluxo <a href="#stream-delete-bytes" id="stream-delete-bytes"></a>

Esta métrica é preenchida toda vez que um fluxo de eventos é excluído, mostrando a soma de todos os bytes excluídos, seja manualmente ou pela data de retenção definida na criação do _event store_.

<figure><img src="../../.gitbook/assets/Stream Delete Bytes (1).png" alt=""><figcaption><p>Métrica de Bytes Excluídos do Fluxo</p></figcaption></figure>

_**Exemplo:** Ao começar a coletar dados para seu event store, você definirá uma data de retenção para os dados. Toda vez que os dados atingirem essa data, seu fluxo de eventos será excluído, ou você também pode excluí-lo manualmente. Neste gráfico, você pode ver que, em algum momento, quase todos os fluxos de eventos foram excluídos._

### Contagem de Exclusões de Fluxo <a href="#stream-delete-count" id="stream-delete-count"></a>

Esta métrica representa a contagem total de fluxos de eventos excluídos. Eles são preenchidos por exclusão por retenção ou exclusão manual.

<figure><img src="../../.gitbook/assets/Stream Delete Count (1).png" alt=""><figcaption><p>Métrica de Contagem de Exclusões de Fluxo</p></figcaption></figure>

_**Exemplo:** Neste gráfico, você pode ver que a contagem de exclusões segue um padrão, mas em algumas datas, uma quantidade menor foi excluída. Isso pode ser devido a uma mudança na data de retenção ou a menos fluxos de eventos habilitados. Excluir dados pode ajudá-lo a mantê-los mais organizados._

### Contagem de Eventos Correspondentes <a href="#matched-events-count" id="matched-events-count"></a>

Esta métrica é preenchida cada vez que um evento corresponde aos critérios do seu pipe de eventos. Uma vez que ele atende à sua configuração, ele coleta dados.

<figure><img src="../../.gitbook/assets/Matched Events Count.png" alt=""><figcaption><p>Métrica de Contagem de Eventos Correspondentes</p></figcaption></figure>

_**Exemplo:** Toda vez que um evento atende aos critérios estabelecidos durante a criação do pipe de eventos, esta métrica será atualizada. É importante monitorar esta métrica, pois ela indica se os critérios estão sendo atendidos corretamente; caso contrário, não haverá dados para coletar. Neste gráfico, você pode ver que em algum momento, atingiu um pico de quase 250.000 eventos. A métrica variará com base no número de campanhas em execução no momento._

### Contagem de Chamadas de Execução de Destino <a href="#target-execution-call-count" id="target-execution-call-count"></a>

Esta métrica é preenchida após o sucesso dos eventos correspondentes. Cada evento correspondente será enviado para uma chamada de execução de destino, de acordo com os critérios estabelecidos. Esta métrica quase sempre seguirá os mesmos parâmetros da contagem de eventos correspondentes.

<figure><img src="../../.gitbook/assets/Target Execution Call Count.png" alt=""><figcaption><p>Métrica de Contagem de Chamadas de Execução de Destino</p></figcaption></figure>

_**Exemplo:** Após um evento corresponder aos critérios, nosso sistema executará o pipe de eventos estabelecido, coletará os dados de acordo com os parâmetros e, em seguida, os enviará para um event store ou webhook, conforme configurado. Neste gráfico, você pode ver a contagem de eventos correspondentes._

### Taxa de Falha na Execução de Destino <a href="#target-execution-failure-rate" id="target-execution-failure-rate"></a>

Esta métrica é preenchida pelas falhas de uma execução de chamada. Se houver algum erro de instabilidade na plataforma ou na configuração do pipe de eventos, nosso sistema preencherá a métrica de taxa de falha.

<figure><img src="../../.gitbook/assets/Target Execution Failure Rate.png" alt=""><figcaption><p>Métrica de Taxa de Falha na Execução de Destino</p></figcaption></figure>

_**Exemplo:** Se uma execução de chamada falhar, verifique a configuração do seu pipe de eventos ou se a plataforma está passando por instabilidade, pois isso pode causar a falha. Neste gráfico, você pode ver que, no período de um mês, houve uma taxa de falha de 1% em um dia, seguida por nenhuma falha depois._
