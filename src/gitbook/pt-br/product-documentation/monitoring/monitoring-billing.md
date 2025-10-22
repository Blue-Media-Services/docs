# Cobranças de Monitoramento

Na aba de monitoramento, serão apresentadas todas as faturas relacionadas ao monitoramento, que estão divididas em 4 subseções.

<figure><img src="../../.gitbook/assets/image (675).png" alt=""><figcaption><p>Subseções de Monitoramento</p></figcaption></figure>

{% hint style="info" %}
_Na BMS, priorizamos a transparência ao exibir cada detalhe de sua fatura. Visite nossa_ [_Página Inicial de Cobrança_](../billing.md) _para entender como as faturas são estruturadas._
{% endhint %}

### Gerenciamento de Pipes de Eventos <a href="#event-pipe-management" id="event-pipe-management"></a>

Toda ação realizada em um pipe de eventos gerará uma requisição. Por exemplo, criar um pipe, listar seus pipes e fazer alterações em um pipe irão, cada um, gerar uma requisição. Além disso, cada pipe de eventos criará registros de eventos por hora, que serão então cobrados com base em um período de 720 horas.

<figure><img src="../../.gitbook/assets/image (671).png" alt=""><figcaption><p>Detalhes do Gerenciamento de Pipes de Eventos</p></figcaption></figure>

_**Exemplo:** Nesta fatura, apenas o pipe de eventos configurado foi cobrado. Observando o número de horas, você pode ver que o pipe esteve ativo por um mês e alguns dias, resultando em uma fatura total de $0,79. Nenhuma outra cobrança ocorreu, pois nenhuma requisição excedeu as primeiras 1.000 requisições gratuitas._

### Gerenciamento de Event Stores <a href="#event-store-management" id="event-store-management"></a>

Na página de _Event Stores_, todas as ações contarão como uma requisição. Se você acessar a página, criar um _event store_, verificar seus fluxos de eventos disponíveis ou baixar um fluxo de eventos, cada uma dessas ações contará como uma requisição. No entanto, o download de um fluxo de eventos também incorrerá em cobranças, assim como o armazenamento de fluxos de eventos. Essas cobranças serão baseadas no tamanho do fluxo de eventos e na duração em que ele é armazenado na BMS.

<figure><img src="../../.gitbook/assets/image (672).png" alt=""><figcaption><p>Detalhes do Gerenciamento de Event Stores</p></figcaption></figure>

_**Exemplo:** Nesta fatura, é possível ver que a maioria das requisições não foi cobrada por não atingir as 1.000 requisições gratuitas. No entanto, as requisições do event store incorreram em uma fatura de $1,95 devido ao alto número de fluxos de eventos gerados dentro daquele event store. Ter um event store configurado também gerou cobranças porque os fluxos de eventos são gerados a cada hora, resultando em uma fatura de $0,47. Adicionalmente, o armazenamento desses fluxos de eventos gerados no servidor da BMS (se o recurso de webhook não for usado) incorreu em uma fatura de $0,04, elevando a fatura total para $2,46._

### Monitoramento de Métricas <a href="#metric-monitoring" id="metric-monitoring"></a>

Todas as métricas em qualquer plataforma incorrem em cobranças e são cruciais para analisar o desempenho e tomar decisões estratégicas com base nos dados coletados. A BMS centraliza as cobranças de cada métrica na plataforma sob a aba de Monitoramento, que é responsável por receber todos os eventos dentro da plataforma.

As métricas são cobradas por ponto registrado e pelos bytes processados pelos servidores da BMS para gerar essas métricas.

<figure><img src="../../.gitbook/assets/image (673).png" alt=""><figcaption><p>Detalhes do Monitoramento de Métricas</p></figcaption></figure>

_**Exemplo:** Nesta fatura, nota-se que quase 17 milhões de pontos de métrica foram acumulados em um mês. Este total é gerado pela soma de todas as métricas na conta do usuário, resultando em um custo de $83,47. Adicionalmente, a quantidade de dados escaneados para gerar essas métricas foi de quase 119 mil GB, resultando em uma cobrança de $2,37, para uma fatura total de $85,84._

### Monitoramento em Tempo Real <a href="#real-time-monitoring" id="real-time-monitoring"></a>

Some products have a real-time tab that displays events from your campaign as they happen. For example, when an ad is displayed, the user's location will be shown based on the ad exchange used, along with additional information. Each time the real-time tab is accessed, it will incur costs.

<figure><img src="../../.gitbook/assets/image (674).png" alt=""><figcaption><p>Detalhes do Monitoramento em Tempo Real</p></figcaption></figure>

_**Exemplo**: Neste caso, as requisições de eventos recentes em tempo real foram relativamente baixas, mas excederam a marca de 100.000 eventos gratuitos, resultando em uma cobrança de $0,14._
