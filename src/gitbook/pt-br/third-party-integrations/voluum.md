# Voluum

Voluum é uma plataforma de análise baseada em nuvem que ajuda profissionais de marketing a monitorar, otimizar e analisar suas campanhas digitais. Ela gerencia grandes volumes de dados e fornece insights em tempo real sobre métricas chave, como cliques, conversões e ROI.

## Rastreando Campanhas na BMS com Voluum <a href="#tracking-bms-campaigns-with-voluum" id="tracking-bms-campaigns-with-voluum"></a>

Ao integrar a BMS com o Voluum, os anunciantes podem exportar dados de campanha, rastrear eventos específicos e obter uma visão mais aprofundada do desempenho de suas campanhas.

<figure><img src="../.gitbook/assets/image (1125).png" alt=""><figcaption><p>Página inicial da Voluum</p></figcaption></figure>

### Rastreando Cliques e Impressões <a href="#tracking-clicks-and-impressions" id="tracking-clicks-and-impressions"></a>

{% hint style="info" %}
_Este artigo se concentra na integração da **BMS** como fonte de tráfego no **Voluum**. Não abordaremos todas as opções de criação de campanhas do Voluum. Para mais detalhes sobre os recursos do Voluum, visite nossa seção de_ [_Informações Adicionais_](voluum.md#informacoes-adicionais) _ou a_ [_documentação do Voluum_](https://doc.voluum.com/)_._
{% endhint %}

Você deve adicionar a BMS como uma fonte de tráfego em suas campanhas do Voluum para extrair dados.

1. Selecione a guia "Campanhas".
2. Clique em "Criar" para criar uma nova campanha.
3.  Selecione "Simples" como modo de criação.\


    <figure><img src="../.gitbook/assets/image (1126).png" alt=""><figcaption><p>Editor de Campanha no Voluum - Aba <em>Geral</em></p></figcaption></figure>


4. Preencha os detalhes:
   * _**Geral**_
     * **Fonte de Tráfego:** Pesquise por "BMS" e selecione-a.
     * **Tipo de Tráfego**: Selecione o tipo de tráfego com base no tipo da sua campanha, como Banner, por exemplo.
     * **Rótulo do País:** Selecione o país onde sua campanha está sendo executada.
     * **Modelo de Custo:** Selecione o modelo de custo aplicado à sua campanha.
5. Depois de estar satisfeito com os demais parâmetros, clique em Salvar para continuar.
6.  Selecione a guia Rastreamento e Automação.\


    <figure><img src="../.gitbook/assets/image (4) (3).png" alt=""><figcaption><p>Editor de Campanhas do Voluum – Guia Rastreamento e Automação</p></figcaption></figure>


7.  Aqui, você encontrará 2 informações primordiais que concluirão o processo de integração:

    * **URL da Campanha:** Este parâmetro permitirá que o Voluum rastreie cliques nas suas campanhas BMS. Use o botão de copiar para copiar este link e depois use-o como o link do seu anúncio, ou seja, cole-o no parâmetro "Link Para" dos seus anúncios ou criativos.

    <figure><img src="../.gitbook/assets/image (1129).png" alt=""><figcaption><p>Editor de Criativos – Link para</p></figcaption></figure>

    * **URL de Clique de Impressão:** Este parâmetro permitirá que o Voluum rastreie impressões nas suas campanhas BMS. Você deve copiá-lo usando o botão de copiar, colar essa URL dentro de uma tag de pixel como fonte e, em seguida, adicionar essa tag de pixel ao código HTML do seu criativo.
      * _**Exemplo:** Este é um exemplo de uma tag de pixel_\
        `<img src="VOLUUM_IMPRESSION_PIXEL_URL" style="position: absolute; opacity: 0;">`\
        &#xNAN;_&#x56;ocê deve substituir o parâmetro 'src' pelo link que você copiou do Voluum. Depois de substituir, o resultado será assim:_\
        `<img src="https://ImpressionURL.copied/from/Voluum" style="position: absolute; opacity: 0;">`

    <figure><img src="../.gitbook/assets/image (1128).png" alt=""><figcaption><p>Editor de Criativos - Aba de Colar HTML</p></figcaption></figure>

## Informações Adicionais <a href="#additional-information" id="additional-information"></a>

Após seguir os passos acima, você começará a receber os dados das suas campanhas BMS no Voluum, e a integração estará completa. Você também pode usar os artigos abaixo para saber mais sobre nosso processo de criação de anúncios e outras funcionalidades do Voluum.

* [Criativos](../product-documentation/ad-server/creatives.md)
* [Anúncios](../product-documentation/ad-server/ads/)
* [Criar uma Campanha no Voluum](https://doc.voluum.com/article/create-a-voluum-campaign)
* [Adicione uma Fonte de Tráfego no Voluum](https://doc.voluum.com/article/add-a-traffic-source-to-voluum)
* [Adicione uma Rede Afiliada no Voluum](https://doc.voluum.com/article/add-an-affiliate-network-to-voluum)
