# Gerenciando Públicos-alvo

Após criar uma Campanha, você precisará definir pelo menos um Público-alvo para executá-la. Públicos-alvo são, basicamente, o tipo de público para o qual você deseja que sua campanha seja exibida. Nossos Públicos-alvo funcionam usando regras "**E**", não "**OU**", então sempre que você inclui um público-alvo, você estará restringindo sua campanha ainda mais para o seu público desejado.

Se você configurar sua campanha com Públicos-alvo mais amplas, seu orçamento será gasto mais rapidamente, pois você receberá requisições de lance de uma vasta gama de _publishers_.

## Predefinição de Públicos-alvo <a href="#pre-targets" id="pre-targets"></a>

Estes são os Públicos-alvo que funcionarão como o primeiro filtro (Localização, _Pools_ de Cookies, _Exchange_) e excluirão outras possibilidades.

_**Exemplo**: Se o seu objetivo é definir um público específico de um Pool de Cookies, seus anúncios serão exibidos apenas para os usuários dentro daquele Pool de Cookies, desconsiderando outros usuários._

## Públicos-alvo <a href="#targets" id="targets"></a>

Você pode escolher para quem exibir os anúncios com base em onde esses usuários estão localizados, especificando o país e a região ou adicionando cercas geográficas (geofences) em torno de endereços específicos.

### Localização <a href="#location" id="location"></a>

<figure><img src="../../.gitbook/assets/image (826).png" alt=""><figcaption><p>Localização</p></figcaption></figure>

* Geografias - Ao selecionar países ou regiões específicas, seus anúncios aparecerão apenas para usuários que acessam dessas localizações geográficas.
* Geofences (Cercas Geográficas) - Ao selecionar países ou regiões específicas, seus anúncios aparecerão apenas para usuários que acessam dessas localizações geográficas.

### Conteúdos - Apenas Sites Web <a href="#contents-only-websites" id="contents-only-websites"></a>

Ao selecionar esta opção de público-alvo, sua segmentação de conteúdo direcionará seus anúncios apenas para sites, o que significa que apenas usuários de sites receberão seus anúncios com base nas seguintes opções de conteúdo.

<figure><img src="../../.gitbook/assets/image (97).png" alt=""><figcaption><p>Conteúdos - Apenas Sites Web</p></figcaption></figure>

* Idiomas - Ao incluir um idioma específico, seus anúncios aparecerão apenas em sites nesse idioma.
* Categories - Ao incluir categorias específicas, seus anúncios aparecerão apenas em sites com conteúdo nessas categorias.
* Impressões Diárias - Defina o número mínimo de impressões diárias que um site deve receber para exibir seus anúncios, garantindo que eles apareçam apenas em sites que atendam ao limite de tráfego exigido.
* Domains - Ao incluir domínios específicos, seus anúncios aparecerão apenas nesses sites especificados.
* Palavras-chave da URL - Ao definir palavras-chave de URL, você pode refinar onde seus anúncios aparecem com base no conteúdo da URL.

### **C**onteúdos - Apenas Aplicativos <a href="#contents-only-apps" id="contents-only-apps"></a>

Ao selecionar esta opção de público-alvo, sua segmentação de conteúdo entregará seus anúncios apenas para aplicativos, o que significa que apenas usuários de aplicativos receberão seus anúncios com base na seleção de apps.

<figure><img src="../../.gitbook/assets/image (99).png" alt=""><figcaption><p>Conteúdos - Apenas Aplicativos</p></figcaption></figure>

* Aplicativos - Ao incluir aplicativos específicos, seus anúncios aparecerão apenas nesses aplicativos especificados. Alternativamente, excluir certos aplicativos garante que seus anúncios não serão exibidos nesses aplicativos, mas permanecerão disponíveis em todos os outros. Se nenhuma preferência de aplicativo for definida, seus anúncios podem ser exibidos em qualquer aplicativo, maximizando o alcance.

{% hint style="info" %}
Por favor, note que só podemos exibir seus anúncios em aplicativos que estão conectados a uma das _Ad Exchanges_ que suportamos.
{% endhint %}

### Conteúdos - Aplicativos e Sites Web <a href="#contents-apps-and-websites" id="contents-apps-and-websites"></a>

Ao selecionar esta opção de público-alvo, sua segmentação de conteúdo entregará seus anúncios a usuários tanto em sites quanto em aplicativos. Nenhuma outra opção de público-alvo está disponível nesta aba quando esta opção é selecionada.

<figure><img src="../../.gitbook/assets/image (100).png" alt=""><figcaption><p>Conteúdos - Aplicativos e Sites Web</p></figcaption></figure>

* A campanha segmentará usuários em sites e aplicativos, garantindo um amplo alcance. As opções de público-alvo não estão disponíveis, o que significa que a campanha será entregue a todos os sites e aplicativos sem filtragem de público. Se desejar especificar seu público-alvo, selecione apenas sites ou apenas aplicativos.

### **Dispositivo** <a href="#device" id="device"></a>

<figure><img src="../../.gitbook/assets/image (98).png" alt=""><figcaption><p>Dispositivo</p></figcaption></figure>

* Sistemas Operacionais - Ao selecionar sistemas operacionais específicos, seus anúncios serão exibidos para usuários que navegam na web nesses sistemas.
* Navegadores - Ao selecionar navegadores específicos, seus anúncios serão exibidos para usuários que navegam na web através desses navegadores.
* Tipos de Dispositivo - Ao selecionar tipos de dispositivo específicos, seus anúncios serão exibidos para usuários que navegam na web nesses dispositivos.
* Cookie Pools - Ao selecionar cookie pools específicos, seus anúncios segmentarão apenas os usuários que foram adicionados a esses _pools_ selecionados.
* Identifier Pools - Ao selecionar identifier pools específicos, seus anúncios segmentarão apenas os usuários que foram adicionados a esses _pools_ selecionados.

### **Inventário** <a href="#inventory" id="inventory"></a>

<figure><img src="../../.gitbook/assets/image (925).png" alt=""><figcaption><p>Inventário</p></figcaption></figure>

* Exchange - Ao selecionar _ad exchanges_ específicas, seus anúncios serão exibidos através dessas plataformas.
* Posições - Selecione posições de inventário específicas para posicionar estrategicamente seus anúncios para ótima visibilidade e engajamento.
* Visibilidade (_Viewability_) - Ajuste o controle deslizante para definir o limite mínimo de visibilidade para os espaços de anúncio. Seus anúncios serão combinados apenas com posições de inventário onde a porcentagem de visibilidade é maior que o limite selecionado.
* Taxa de Cliques (CTR) - Ajuste o controle deslizante para definir o limite mínimo de Taxa de Cliques para os espaços de anúncio. Seus anúncios serão combinados apenas com inventários onde o CTR é maior que o limite selecionado. A informação usada para este recurso é o banco de dados da BMS, de acordo com todas as campanhas em execução que coletam dados. Este recurso funciona para os inventários de todas as _exchanges_.

## Usando IA para definir Públicos-alvo <a href="#using-ai-to-define-targets" id="using-ai-to-define-targets"></a>

Atualmente, nossa plataforma não possui recursos nativos de IA. No entanto, sinta-se à vontade para usar qualquer ferramenta de IA para analisar seus dados e definir seu público-alvo. Aqui estão alguns exemplos de _prompts_ que você pode usar com a IA de sua escolha:

_**Exemplo de Prompt 1**: "Com base nos dados fornecidos, em quais domínios devo focar minhas campanhas se meu objetivo é aumentar a taxa de cliques?"_

_**Exemplo de Prompt 2**: "Com base nos dados fornecidos, em quais localidades minhas campanhas serão mais eficazes?"_

_**Exemplo de Prompt 3**_: "Quais domínios, com base nos dados fornecidos, devo colocar na lista de exclusão (_blacklist_) para aumentar a taxa de cliques de minhas campanhas?"

A IA pode auxiliar na definição de públicos-alvo alinhados com seus objetivos. Ao analisar os valores do público-alvo, você obtém insights para ajustes de campanha. Por exemplo, a IA pode utilizar dados do nosso produto de Monitoramento, com base nos resultados e objetivos de sua campanha, apresentando possíveis mudanças para sua otimização. Por exemplo, ao usar um Pipelines de Eventos para cliques em anúncios (ADS - Clicked), você pode obter dados sobre quais domínios estão recebendo mais cliques, permitindo obter mais insights a partir dessa informação.

## Criando um Público-alvo <a href="#creating-a-target" id="creating-a-target"></a>

{% hint style="info" %}
**Antes de começar!** É possível selecionar quantos filtros desejar em um único público-alvo. No entanto, tenha em mente que a dificuldade de encontrar uma correspondência com um _publisher_ aumentará à medida que você adicionar mais filtros. Você também pode definir mais de um público-alvo com filtros diferentes e executar sua campanha para cada um separadamente.
{% endhint %}

Na página da Campanhas, após ter selecionado uma campanha, pressione <img src="../../.gitbook/assets/image (158).png" alt="Create Target" data-size="line"> para começar a criar seu público-alvo.

<figure><img src="../../.gitbook/assets/image (103).png" alt=""><figcaption><p>Seção de Público-alvo</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (157).png" alt="" width="563"><figcaption><p>Editor de Públicos-alvo</p></figcaption></figure>

Ao adicionar públicos-alvo, preste atenção aos sinais de <img src="../../.gitbook/assets/image (471).png" alt="Check" data-size="original"> e <img src="../../.gitbook/assets/image (472).png" alt="Exclude" data-size="line">. Eles indicam se você está selecionando ou excluindo um filtro para sua campanha. Os filtros que você escolher serão **listados** em seu filtro de público-alvo, mostrando o que será incluído ou excluído daquele público-alvo específico.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-21 073343.png" alt=""><figcaption><p>Seleção ou Exclusão no Público-alvo</p></figcaption></figure>

Após selecionar e configurar seu público-alvo, clique em ![](<../../.gitbook/assets/image (762).png>).

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-21 073834.png" alt=""><figcaption><p>Tela de Público-alvo Configurada</p></figcaption></figure>

Você pode adicionar quantos públicos-alvo forem necessários à sua campanha e pode livremente ativar ou desativar cada público-alvo durante a campanha para ajustá-lo às suas necessidades.

<figure><img src="../../.gitbook/assets/image (102).png" alt=""><figcaption><p>Lista de Públicos-alvo</p></figcaption></figure>

## Impressões Estimadas <a href="#estimated-impressions" id="estimated-impressions"></a>

Ao criar um público-alvo, você notará que, para a maioria das opções de público-alvo disponíveis, há uma estimativa de quantas impressões podem ser alcançadas diariamente. Essa estimativa representa a mediana das impressões diárias nos últimos 7 dias.

{% hint style="info" %}
Este recurso funciona apenas com inclusões e ainda não está disponível para Palavras-chave de URL.
{% endhint %}

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-21 075508.png" alt=""><figcaption><p>Impressões Estimadas</p></figcaption></figure>

_**Exemplo**: Na imagem acima, você notará que para cada idioma, a estimativa de impressões é mostrada na mesma linha do idioma. Neste exemplo, selecionar Inglês e Português trará aproximadamente 5,8 milhões de impressões para Inglês e aproximadamente 2,4 milhões de impressões para Português._

Uma vez que você selecione múltiplas opções dentro de um filtro, o número de impressões será somado. Após fechar o grupo de edição, a soma total será exibida.

<figure><img src="../../.gitbook/assets/image (839).png" alt=""><figcaption><p>Impressões Estimadas - Soma Total</p></figcaption></figure>

_**Exemplo**: Na imagem acima, você notará que Inglês e Português foram selecionados como idiomas para este público-alvo, e suas impressões estimadas foram somadas quando o grupo foi fechado, resultando em uma estimativa total de 101,5M de impressões para ambos os idiomas combinados. Categories e Domains também foram selecionados. Em Categories, você verá que várias categorias foram selecionadas, resultando em 165,9M de impressões quando combinadas. Para Domains, cada domínio que você inclui se soma ao total de impressões. Neste caso, apenas dois domínios foram selecionados, resultando em uma média de 9,2M de impressões._

## Habilitando e Desabilitando um Público-alvo <a href="#enabling-and-disabling-a-target" id="enabling-and-disabling-a-target"></a>

Para iniciar uma campanha e usar seu público-alvo configurado, garanta que os públicos-alvo estejam habilitadas. Se precisar modificar ou simplesmente parar de usar um público-alvo específico, você pode desabilitá-lo, e a campanha deixará de usar esse público-alvo imediatamente.

<figure><img src="../../.gitbook/assets/image (755).png" alt=""><figcaption><p>Botões de Habilitar/Desabilitar</p></figcaption></figure>

## Duplicando um Público-alvo <a href="#duplicating-a-target" id="duplicating-a-target"></a>

Se você quiser reutilizar um público-alvo denso, mas com poucas alterações, tem a opção de duplicar esse público-alvo e economizar tempo. Simplesmente clique em <img src="../../.gitbook/assets/image (209).png" alt="Duplicate Target" data-size="line"> para duplicar seu público-alvo, e uma cópia desse público-alvo será criado instantaneamente.

## Ações em Lote <a href="#bulk-actions" id="bulk-actions"></a>

Se você selecionar mais de um público-alvo, é possível realizar ações em lote.

Após selecionar dois ou mais públicos-alvo, o botão de ações em lote será habilitado. Então, após clicar no menu <img src="../../.gitbook/assets/image (753).png" alt="Bulk Actions" data-size="line">, serão mostradas três possibilidades: **Habilitar**, **Desabilitar** e **Excluir** públicos-alvo em lote. Isso ajuda você a realizar mais ações de uma só vez.

## Excluindo um Público-alvo <a href="#deleting-a-target" id="deleting-a-target"></a>

Se um público-alvo não for mais útil para sua campanha, você pode clicar em <img src="../../.gitbook/assets/image (210).png" alt="Delete Target" data-size="line"> para excluir permanentemente o público-alvo, e uma tela de confirmação será mostrada a você.

<figure><img src="../../.gitbook/assets/image (754).png" alt=""><figcaption><p>Exclusão de Público-alvo</p></figcaption></figure>

{% hint style="danger" %}
_Atenção! Sempre aconselhamos desabilitar o público-alvo previamente e analisar se é necessário excluí-lo ou simplesmente modificá-lo, pois esta ação não pode ser desfeita._
{% endhint %}
