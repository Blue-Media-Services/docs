---
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Instruções de Instalação

Após configurar eventos e ações para o seu rastreador, você deve instalá-lo em seu site. Isso pode ser feito seguindo as instruções na aba de instruções de instalação.

<figure><img src="../../../.gitbook/assets/image (1085).png" alt=""><figcaption><p>Instruções de Instalação</p></figcaption></figure>

Para acessar a aba de instruções dos rastreadores, selecione o rastreador que você precisa instalar na lista de rastreadores. Você deve escolher apenas um rastreador por vez para usar esta aba. A aba conterá uma seção para cada evento criado para o rastreador selecionado.

Existem alguns métodos de instalação disponíveis para este recurso: _Script_, _Pixel_, _Redirecionamento,_ _AppsFlyer e Template de Rastreamento do Google Ads_. Após expandir a seção do evento que deseja instalar, você pode escolher uma destas opções:

## Script

O rastreamento baseado em _script_ usa trechos de código (_code snippets_) embutidos nas páginas de um site para capturar as interações do usuário. O _script_ coleta dados sobre cliques, tempo gasto nas páginas e ações específicas realizadas pelos visitantes. No entanto, ele exige que os navegadores dos usuários tenham o JavaScript habilitado; caso contrário, não funcionará.

Eventos e ações são contados toda vez que o _script_ carrega, portanto, ele deve ser instalado em páginas específicas com base no que você pretende rastrear. Para simplificar o processo de instalação, você também pode usar gerenciadores de tags como o Google Tag Manager (GTM).

Estas são algumas vantagens de usar o método _Script_:

* **Dados Valiosos**: Rastreia comportamentos detalhados do usuário, como cliques, tempo gasto na página e caminhos de navegação.
* **Análise em Tempo Real**: Fornece _insights_ imediatos sobre a atividade do usuário enquanto ela acontece.

### Casos de Uso <a href="#use-cases" id="use-cases"></a>

O rastreamento por _script_ coleta o comportamento detalhado do usuário diretamente do seu site, ajudando a otimizar campanhas e a melhorar o desempenho de marketing. Abaixo estão as principais aplicações deste método:

* **Desempenho da Landing Page**: Uma empresa de Software como Serviço (SaaS) pode usar um _script_ para monitorar como os usuários interagem com os CTAs em uma _landing page_, otimizando as taxas de conversão.
* **Análise da Jornada do Usuário**: Uma loja de e-commerce pode rastrear a navegação do cliente desde as páginas de produto até o checkout, identificando pontos de abandono.
* **Medição do ROI da Campanha**: Uma agência de marketing digital pode instalar _scripts_ nos sites dos clientes para rastrear o tráfego de campanhas PPC e atribuir conversões.

### Como Instalar <a href="#how-to-install" id="how-to-install"></a>

1. Na página de Rastreadores da BMS, clique na aba Instruções de Instalação.
2. Selecione a opção Usar Script.
3. Use o botão ![](<../../../.gitbook/assets/image (3).png>) para copiar o _script_ exibido.
4. Se você configurou campos de dados personalizados, use a seção indicada em vermelho para informar os valores dos dados personalizados.
5. Cole o código em seu site, precisamente na página onde você deseja que este evento seja capturado.

<figure><img src="../../../.gitbook/assets/image (1086).png" alt=""><figcaption><p>Script</p></figcaption></figure>

## Pixel

O rastreamento por _pixel_ envolve o uso de uma imagem invisível ou código embutido em páginas da web ou e-mails. Quando um usuário acessa o conteúdo, o _pixel_ renderiza e envia de volta informações como o endereço IP do usuário, tipo de dispositivo e ações realizadas. Este método é amplamente utilizado em campanhas de marketing para medir conversões e desempenho de anúncios.

Eventos e ações são rastreados cada vez que o _pixel_ renderiza, portanto, ele deve ser instalado em páginas ou e-mails específicos com base no que você pretende monitorar. Para simplificar o processo de instalação, você pode usar gerenciadores de tags como o Google Tag Manager (GTM).

Estas são algumas vantagens de usar o método _Pixel_:

* **Integração com E-mail e Web**: Funciona perfeitamente em e-mails e páginas da web para rastrear aberturas, cliques e conversões.
* **Retargeting Preciso**: Captura dados para criar públicos de _retargeting_ e melhorar a relevância de sua campanha de anúncios.

### Casos de Uso <a href="#use-cases" id="use-cases"></a>

O rastreamento por _pixel_ coleta dados de e-mails e sites, permitindo uma análise precisa da campanha e _retargeting_. Aqui estão alguns exemplos práticos de marketing:

* **Rastreamento de Campanha de E-mail**: Um serviço de assinatura pode embutir um _pixel_ em e-mails promocionais para medir taxas de abertura e cliques em ofertas de desconto.
* **Retargeting de Anúncios**: Uma marca de cosméticos pode usar um _pixel_ para fazer _retargeting_ de usuários que visualizaram um produto, mas não concluíram a compra, mostrando-lhes anúncios personalizados.
* **Otimização da Geração de Leads**: Uma agência imobiliária pode instalar um _pixel_ em sua página de envio de formulário para rastrear os _leads_ gerados a partir de campanhas de anúncios específicas.

### Como Instalar <a href="#how-to-install" id="how-to-install"></a>

1. Na página de Rastreadores da BMS, clique na aba Instruções de Instalação.
2. Selecione a opção Usar Pixel.
3. Use o botão <img src="../../../.gitbook/assets/image (4).png" alt="" data-size="line"> para copiar a _tag_ de imagem exibida.
4. Se você configurou campos de dados personalizados, use a seção indicada em vermelho para informar os valores.
5. Cole o código em seu site, ou e-mail, precisamente onde você deseja que este evento seja capturado.

<figure><img src="../../../.gitbook/assets/image (1087).png" alt=""><figcaption><p>Pixel</p></figcaption></figure>

## Redirecionamento <a href="#redirect" id="redirect"></a>

O rastreamento por redirecionamento de URL funciona enviando os usuários através de um link intermediário antes de chegarem ao destino final. Este passo intermediário coleta dados valiosos, como fontes de tráfego, parâmetros de campanha e comportamento do usuário. É um método prático para rastrear cliques e entender o desempenho de campanhas externas ou links de afiliados.

Estas são algumas vantagens de usar o método Redirecionamento:

* **Atribuição Eficaz**: Rastreia com precisão as fontes de tráfego e o desempenho de afiliados.
* **Insights Específicos da Campanha**: Ideal para medir o sucesso de campanhas externas ou de afiliados.

### Casos de Uso <a href="#use-cases" id="use-cases"></a>

O rastreamento por redirecionamento de URL simplifica o monitoramento de desempenho ao capturar dados através de links intermediários. Veja como ele aprimora os esforços de marketing:

* **Marketing de Afiliados**: Um provedor de VPN pode oferecer a influenciadores links de redirecionamento únicos para rastrear assinaturas e recompensar os parceiros de melhor desempenho.
* **Comparação de Plataformas de Anúncios**: Uma marca de fitness pode usar links de redirecionamento em diferentes plataformas de anúncios para determinar qual plataforma gera mais inscrições.
* **Eficácia de Campanha de E-mail**: Uma plataforma de educação online pode incluir links de redirecionamento em CTAs de e-mail para rastrear quantos usuários se inscrevem em cursos através da campanha.

### Como Instalar <a href="#how-to-install" id="how-to-install"></a>

1. Na página de Rastreadores da BMS, clique na aba Instruções de Instalação.
2. Selecione a opção Usar Redirecionamento.
3. Informe a URL para onde você deseja redirecionar o usuário após o evento ser capturado.
4. Use o botão ![](<../../../.gitbook/assets/image (5).png>) para copiar a URL exibida.
5. Use a URL gerada da mesma forma que usaria a URL que você forneceu.

<figure><img src="../../../.gitbook/assets/image (1088).png" alt=""><figcaption><p>Redirecionamento</p></figcaption></figure>

Após instalar os rastreadores de seus eventos, você deve começar a receber dados deles. É possível acompanhar este processo na aba de métricas.

## AppsFlyer

AppsFlyer é uma plataforma de atribuição móvel e análise de marketing. Ela permite que as empresas meçam e analisem o desempenho de suas campanhas de publicidade móvel, atribuindo instalações de aplicativos, eventos no aplicativo e conversões aos respectivos canais de marketing ou campanhas responsáveis por gerá-los.

<figure><img src="../../../.gitbook/assets/image (1116).png" alt=""><figcaption><p>AppsFlyer</p></figcaption></figure>

A plataforma também oferece soluções de atribuição precisas, permitindo que os profissionais de marketing identifiquem as fontes de instalações de aplicativos, eventos no aplicativo e conversões — seja da rede BMS, de outros canais de anúncios ou de fontes orgânicas.

Estas são algumas vantagens de integrar a BMS com o AppsFlyer:

* **Insights Poderosos**: Obtenha acesso a dados detalhados sobre o comportamento do usuário, desempenho da campanha, retorno sobre o investimento (ROI) e valor do ciclo de vida do cliente (LTV).
* **Casos de Uso**: Suporta uma variedade de cenários, incluindo a otimização de campanhas de marketing, a melhoria de estratégias de aquisição de usuários e o aprimoramento dos esforços de retenção.

### Casos de Uso <a href="#use-cases" id="use-cases"></a>

O AppsFlyer é uma plataforma que rastreia as interações do usuário e o desempenho da campanha para aplicativos, fornecendo _insights_ chave para otimizar estratégias de marketing. Aqui estão seus principais casos de uso:

* **Atribuição de Instalações de App**: O AppsFlyer pode rastrear quais campanhas geram mais instalações de aplicativos, ajudando os profissionais de marketing a alocar orçamentos para os canais mais eficazes.
* **Rastreamento de Eventos no App**: O AppsFlyer pode monitorar as ações do usuário dentro do aplicativo, como compras ou visualizações de conteúdo, fornecendo _insights_ para otimizar o engajamento do usuário.
* **Detecção de Fraude**: As ferramentas antifraude do AppsFlyer podem detectar e prevenir instalações ou cliques fraudulentos, garantindo um desempenho de campanha confiável e protegendo o ROI.

### Como integrar a BMS com sua conta AppsFlyer <a href="#how-to-integrate-bms-with-your-appsflyer-account" id="how-to-integrate-bms-with-your-appsflyer-account"></a>

Depois de criar sua conta e configurar seu aplicativo no AppsFlyer, é hora de adicionar a BMS como um parceiro de _marketplace_ para enviar os dados do seu aplicativo para nossa plataforma. Na página inicial do AppsFlyer, navegue até o menu à esquerda, clique em Collaborate e, em seguida, selecione Partner Marketplace.

<figure><img src="../../../.gitbook/assets/image (1165).png" alt=""><figcaption><p>AppsFlyer Partner Marketplace</p></figcaption></figure>

1.  Procure por Blue Media Services LTDA usando a barra de pesquisa e selecione esta opção na lista de resultados.\


    <figure><img src="../../../.gitbook/assets/Captura de tela 2024-12-17 082704.png" alt=""><figcaption><p>BMS Partner Marketplace</p></figcaption></figure>
2.  Clique em <img src="../../../.gitbook/assets/image (1166).png" alt="" data-size="line"> para começar a configurar a integração.\


    <figure><img src="../../../.gitbook/assets/image (1167).png" alt=""><figcaption><p>Gerenciador de Integração</p></figcaption></figure>
3. Ative a chave seletora <img src="../../../.gitbook/assets/image (1168).png" alt="" data-size="line">.
4. _Postbacks_ padrão são _postbacks_ de atribuição enviados para ações do usuário, como instalação, reinstalação, etc. Selecione como enviar os _postbacks_ configurados para nossa plataforma.
5. Postbacks de eventos no aplicativo: Ative esta chave seletora para nos enviar os dados de seus eventos no aplicativo, como adicionar ao carrinho, produto visualizado, entre outros.
6. Janela de postback de eventos no aplicativo: Defina o período após uma instalação, reatribuição ou reengajamento durante o qual os _postbacks_ de eventos no aplicativo serão enviados para nossa plataforma.
7. Clique em <img src="../../../.gitbook/assets/image (1169).png" alt="" data-size="line"> para começar a adicionar um evento.
8. Preencha as informações:
   * **Evento do AppsFlyer**: Defina um nome para o seu evento.
   * **Evento do parceiro mapeado**: Copie e cole o código BRN da aba de instruções de instalação dos rastreadores da BMS, no 3º passo.
   * **Para usuários de**: Selecione "This partner only" no menu suspenso.
   * **Incluindo**: Selecione "Value & no revenue" no menu suspenso.
9. Adicione quantos eventos precisar.
10. Clique em <img src="../../../.gitbook/assets/image (1170).png" alt="" data-size="line"> para salvar sua integração.

Após completar estes passos, a BMS estará integrada com sua conta AppsFlyer, e os dados de eventos do seu aplicativo começarão a ser enviados para nossa plataforma.

## Template de Rastreamento do Google Ads

O _Google Tag Manager_ (GTM) é uma ferramenta que centraliza e simplifica a instalação de códigos de rastreamento em um site sem a necessidade de alterações diretas no código-fonte. Em vez de inserir cada script manualmente, você só precisa instalar o contêiner do GTM uma vez e, a partir daí, gerenciar todos os rastreamentos, pixels e eventos pelo painel do GTM.

O GTM funciona disparando trechos de código de rastreamento com base nas regras que você configura (chamadas de gatilhos). Isso permite decidir quais páginas ou ações do usuário ativarão cada tag.

Essa abordagem elimina a necessidade de constantes edições no código, tornando o processo mais eficiente e seguro.

Aqui estão algumas vantagens de usar rastreamentos através do GTM:

* **Gerenciamento Centralizado:** Todos os scripts de rastreamento e pixels são controlados em um único lugar.
* **Flexibilidade:** Configure gatilhos condicionais, como cliques em botões, visualizações de páginas ou envio de formulários.
* **Menor Dependência Técnica:** As equipes de marketing podem gerenciar tags sem precisar recorrer a desenvolvedores para cada atualização.
* **Escalabilidade:** Perfeito para sites que executam várias campanhas, já que simplifica a implementação e manutenção.

### Casos de Uso <a href="#use-cases" id="use-cases"></a>

O rastreamento com o GTM aprimora os insights sobre o comportamento do usuário e o desempenho das campanhas, como por exemplo:

* **Rastreamento de Conversão:** Uma loja online pode configurar um evento no GTM que dispara quando uma compra é concluída, garantindo uma atribuição precisa do ROI.
* **Teste de Elementos da Página:** Um site de notícias pode rastrear quais manchetes os usuários mais clicam, otimizando o engajamento com o conteúdo.
* **Mensuração de Campanhas Multicanal:** Uma agência de marketing pode instalar diversos pixels de anúncios (Google Ads, Facebook Ads, LinkedIn Ads) via GTM sem alterar o código do site do cliente.

### Como Instalar <a href="#how-to-install" id="how-to-install"></a>

1. Acesse seu GTM e clique em **Adicionar uma Nova Tag**.
   1. No menu à esquerda, clique em **Tags**.
   2. Clique em **Novo** e dê um nome à sua tag como preferir.
   3. Clique em **Configuração da Tags** e escolha **HTML Personalizado (**_**Custom HTML**_**)**.
2. Adicione o Script de Rastreamento.
   1.  Copie e cole o script exibido nas instruções de instalação.\


       <figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Modelo de Script do Rastreamento do Google Ads</p></figcaption></figure>
   2. Substitua as seções pelos seus valores personalizados:
      * `REPLACE_WITH_PRICE` → o valor da transação (se aplicável).
      * `REPLACE_WITH_QUANTITY` → o número de itens (se aplicável).
      * `REPLACE_WITH_DEDUPLICATIONID` → um ID único da transação ou evento para evitar duplicados.
      *   `{lpurl}` → deixe como está, ele irá resolver automaticamente a URL da landing page.


3. Definir o Gatilho
   1. Em **Desencadeando**, clique em **+** para adicionar um novo gatilho.
   2. Selecione _**Evento personalizado**_.
   3. Insira o nome do evento que corresponde ao evento enviado para o `dataLayer`.
      * Exemplo: se seus desenvolvedores estiverem enviando `dataLayer.push({ event: "purchase" })`, use `purchase` como nome do gatilho.\

   4. Salve o gatilho.
4. Salvar e Publicar
   1. Salve sua nova tag.
   2. Clique em **Salvar** no canto superior direito.
   3. Adicione um nome para a versão (ex.: Tag de Rastreador Adicionado) e clique em **Salvar**.

### Informações Adicionais <a href="#additional-information" id="additional-information"></a>

Confira algumas referências externas que podem ajudá-lo no processo de configuração do aplicativo e integração de parceiros:

* [Primeiros passos - Onboarding para profissionais de marketing](https://support.appsflyer.com/hc/pt/articles/207033486-Primeiros-passos-Onboarding-para-profissionais-de-marketing)
* [Primeiros passos - Integraçao de agências](https://support.appsflyer.com/hc/pt/articles/360002381617-Primeiros-passos-integra%C3%A7%C3%A3o-de-ag%C3%AAncias)
* [Configure um parceiro integrado](https://support.appsflyer.com/hc/pt/articles/4410395957521-Configure-um-parceiro-integrado)
