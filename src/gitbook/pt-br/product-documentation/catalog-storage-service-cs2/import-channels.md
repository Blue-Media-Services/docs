# Canais de Importação

Use canais de importação para carregar o _feed_ do catálogo de seus produtos para nossa plataforma. Este recurso também manterá seu catálogo atualizado de acordo com o _feed_.

## Gerenciando Canais de Importação <a href="#managing-import-channels" id="managing-import-channels"></a>

<figure><img src="../../.gitbook/assets/image (119).png" alt=""><figcaption><p>Lista de Canais de Importação</p></figcaption></figure>

### Criando um Canal de Importação <a href="#creating-an-import-channel" id="creating-an-import-channel"></a>

Para começar a criar um Canal de Importação, primeiro devemos criar o catálogo que conterá os produtos importados pelo _feed_. Para criar um catálogo, siga os passos no artigo de [Catálogos](catalogs.md). Também precisaremos ter um _feed_ de produtos para usar como fonte para nosso canal de importação.

{% hint style="info" %}
Os Canais de Importação podem importar dados de sites HTTP, FTP ou SFTP. O formato XML do Google Merchant é o padrão para criar catálogos e o mais fácil de trabalhar, mas o canal de importação pode ser configurado para usar CSV ou outros formatos XML.
{% endhint %}

1. Clique em <img src="../../.gitbook/assets/image (121).png" alt="" data-size="line"> para começar a criar seu Canal de Importação.
2.  Preencha as informações solicitadas nas 3 abas:\


    <figure><img src="../../.gitbook/assets/image (124).png" alt=""><figcaption><p>Editor de Canal de Importação</p></figcaption></figure>

    1.  Aba Geral

        Nesta aba, você encontrará os detalhes gerais relacionados ao seu canal de importação. Use os exemplos para ajudá-lo a preencher todos os detalhes.

        * Nome: Defina um nome para o seu Canal de Importação.
        * Tags: Defina tags para sua organização.
        * Catálogo: Selecione o catálogo que você criou para receber os produtos do _feed_.
        * Quando criar ou atualizar produtos: Defina o período em que seus produtos serão criados ou atualizados.
        * Quando remover produtos:&#x20;
          * Nunca: Produtos criados ou atualizados na origem serão modificados ou adicionados ao catálogo. No entanto, produtos excluídos na origem não serão removidos do catálogo.
          * Antes de cada importação: Todos os produtos serão excluídos do catálogo antes de cada processo de importação. Em seguida, os produtos que existem na origem serão adicionados ao catálogo. Cuidado! O catálogo permanecerá vazio até que a importação seja concluída, o que pode resultar em banners de anúncios vazios durante este período. Todas as métricas de produtos serão preservadas.
          * Horas após ser importado: Defina quanto tempo após a importação os produtos devem permanecer no catálogo se não forem reimportados. Contanto que a frequência de importação seja menor que o tempo de expiração do produto, o catálogo не ficará vazio. Todas as métricas de produtos serão preservadas.
    2.  Aba Fonte\
        Esta aba contém os detalhes da fonte relacionados ao seu canal de importação. Use os exemplos para ajudá-lo a preencher esses detalhes de acordo com sua opção de fonte.

        * Protocolo: Selecione o protocolo de sua fonte e preencha os detalhes de acordo com sua escolha.
          1.  HTTP:

              <div align="center" data-full-width="false"><figure><img src="../../.gitbook/assets/Captura de tela 2024-08-27 121710.png" alt=""><figcaption><p>Aba Fonte - HTTP</p></figcaption></figure></div>

              * URL: Informe a URL do seu _feed_.
          2.  SFTP e FTP:

              <figure><img src="../../.gitbook/assets/Captura de tela 2024-08-22 090041.png" alt=""><figcaption><p>Aba Fonte - SFTP/FTP</p></figcaption></figure>

              * Host: Informe o host da sua fonte.
              * Porta: Informe a porta da sua fonte.
              * Usuário: Informe um usuário para acessar sua fonte.
              * Senha: Informe a senha para validar seu usuário na fonte.
              * Caminho: Informe o caminho para sua fonte.
        *   Testar Fonte: Este botão, <img src="../../.gitbook/assets/image (991).png" alt="" data-size="line">, permite que você teste sua fonte e recupere dados relevantes para os próximos campos. Existem três abas para o resultado do teste da fonte:

            * Registros Detectados: Exibe os registros do seu _feed_ em formato de tabela.
            * Problemas: Exibe os problemas que podem afetar seu _job_ de importação.
            * Bruto (_Raw_): Exibe o código-fonte do seu arquivo de _feed_.&#x20;

            <figure><img src="../../.gitbook/assets/image (990).png" alt=""><figcaption><p>Resultado do Teste da Fonte</p></figcaption></figure>

        Após terminar o teste, clique em <img src="../../.gitbook/assets/image (992).png" alt="" data-size="line"> para fechar a janela de resultados e preencher automaticamente os próximos campos.

        * Charset: Informe o _charset_ da fonte, que foi previamente detectado no resultado do teste.
        * Formato do Arquivo: O resultado do teste preencherá estes campos automaticamente, mas você pode alterá-los manualmente. Selecione entre estas opções:
          * CSV: _Feed_ de origem baseado em um arquivo com valores separados por vírgula.
            * Delimitador: insira o caractere que separa os valores do seu arquivo.
          * XML: _Feed_ de origem baseado em um arquivo XML.
            * Tag do Item: insira a tag do item em seu arquivo XML.
    3.  Aba Mapeamento\
        Você encontrará nesta aba os detalhes de mapeamento relacionados ao seu canal de importação.

        *   Formato do Template: Selecione entre estas duas opções:

            * Google Shopping: Selecione esta opção se estiver usando um _Feed_ do Google Shopping.

            <figure><img src="../../.gitbook/assets/image (987).png" alt=""><figcaption><p>Aba Mapeamento - Google Shopping</p></figcaption></figure>

            * Avançado: Para qualquer outro tipo de arquivo de _feed_, selecione esta opção.

            <figure><img src="../../.gitbook/assets/image (989).png" alt=""><figcaption><p>Aba Mapeamento - Advanced</p></figcaption></figure>
        * Detectar Template: Clique em <img src="../../.gitbook/assets/image (994).png" alt="" data-size="line">para detectar o melhor _template_ com base no seu arquivo de _feed_.
        * Testar Template: Clique em <img src="../../.gitbook/assets/image (997).png" alt="" data-size="line"> para acessar uma pré-visualização de como seus produtos serão exibidos em seu catálogo. Se houver falhas no mapeamento ou no arquivo de _feed_, você as notará neste teste.

        <figure><img src="../../.gitbook/assets/Captura de tela 2024-09-18 145710.png" alt=""><figcaption><p>Resultado do Teste de Mapeamento</p></figcaption></figure>

        * Clique em <img src="../../.gitbook/assets/image (999).png" alt="" data-size="line"> para prosseguir.
    4.  Aba Filtros\
        Nesta aba, você poderá definir filtros para selecionar os produtos que precisa importar. Isso pode ser útil para reduzir os custos dos _jobs_ de importação, importando apenas os produtos que você precisa.

        * Caminho: Informe um valor de caminho, como um dos rótulos de coluna do _feed_.
        * Operador: Selecione um dos valores de operador; este valor estabelecerá o filtro.
        * Valor: Informe o valor que você precisa filtrar do _feed_ do seu catálogo, como um nome de marca ou um intervalo de IDs de produto.
        * Após preencher os campos, você também precisará inserir os mesmos dados no template exibido. Você deve alterar apenas os valores que está filtrando, caso contrário, não funcionará corretamente.

        Você pode adicionar quantos filtros forem necessários clicando em <img src="../../.gitbook/assets/image (1083).png" alt="" data-size="original">, e também removê-los clicando em ![](<../../.gitbook/assets/image (1084).png>) na mesma linha do filtro que deseja excluir.



        <figure><img src="../../.gitbook/assets/Captura de tela 2024-12-19 110001.png" alt=""><figcaption><p>Aba Filtros</p></figcaption></figure>

        * _**Exemplo 1**: Nesta imagem, você notará que um filtro foi estabelecido usando a coluna description do arquivo de feed como referência para o caminho, o operador escolhido foi 'Contém', e o Valor foi 'Cerdo', significando que este canal de importação só importará produtos que contenham a palavra 'Cerdo' em sua descrição. Você também notará que no template, o conteúdo da linha 'description' foi modificado para corresponder ao valor do filtro._
        * _**Exemplo 2**: Você também notará um filtro usando a coluna 'url' como referência para o caminho; este foi adicionado manualmente. Para adicionar novas colunas manualmente aos seus filtros, elas também devem estar presentes no mapeamento do seu feed. Você também precisa respeitar a semântica do template: colunas são separadas por vírgula, e dois pontos são usados para separar o rótulo de uma coluna de seu valor. Rótulos e valores de colunas devem ser declarados entre aspas._
3. Uma vez que tenha finalizado os passos acima, verifique suas configurações para garantir que tudo está correto, então clique em <img src="../../.gitbook/assets/image (126).png" alt="" data-size="line"> para salvar seu Canal de Importação.
4.  Clique em <img src="../../.gitbook/assets/image (111).png" alt="" data-size="original"> para iniciar um _job_ manual de importação de seus produtos:\


    <figure><img src="../../.gitbook/assets/image (113).png" alt=""><figcaption><p>Tela de Iniciar Jobs</p></figcaption></figure>
5. Clique em <img src="../../.gitbook/assets/image (114).png" alt="" data-size="line"> para começar a importar seus produtos.
6.  Também é possível importar apenas alguns produtos para testar se tudo funciona bem antes de iniciar a importação completa. Podemos fazer isso marcando a caixa 'Modo de Teste', preenchendo os detalhes e clicando em <img src="../../.gitbook/assets/image (115).png" alt="" data-size="line">.\


    <figure><img src="../../.gitbook/assets/image (484).png" alt=""><figcaption><p>Tela de Iniciar Jobs - Modo de Teste</p></figcaption></figure>
7.  Acompanhe sua importação na aba Jobs. Nesta aba, podemos ver os problemas com nossa importação ou se foram concluídas. É possível entender o problema clicando em  ![](<../../.gitbook/assets/image (347).png>) ou ![](<../../.gitbook/assets/image (348).png>) na mesma linha do _job_ que falhou.\


    <figure><img src="../../.gitbook/assets/image (345).png" alt=""><figcaption><p>Aba Jobs</p></figcaption></figure>

### Editando um Canal de Importação <a href="#editing-an-import-channel" id="editing-an-import-channel"></a>

Podemos editar nossos canais de importação clicando em <img src="../../.gitbook/assets/image (116).png" alt="" data-size="line"> na mesma linha do canal que você precisa editar. Todos os detalhes estão disponíveis para edição.

### Excluindo um Canal de Importação <a href="#deleting-an-import-channel" id="deleting-an-import-channel"></a>

Podemos excluir canais de importação não utilizados clicando em <img src="../../.gitbook/assets/image (118).png" alt="" data-size="line"> na mesma linha do canal a ser excluído. No entanto, isso também excluirá as métricas relacionadas a ele, então proceda com cautela. Alternativamente, também podemos arquivar esses canais clicando em <img src="../../.gitbook/assets/image (117).png" alt="" data-size="line"> Para visualizar canais de importação arquivados, ative a opção 'Arquivados' acima da lista.

## Aba de Métricas <a href="#metrics-tab" id="metrics-tab"></a>

A aba de métricas dos canais de importação contém dados sobre seus _jobs_ de importação, como processamento de dados, desempenho e taxa de falha. A aba exibirá dados de toda a conta para todos os canais se nenhum canal for selecionado. Selecionar um único canal mostrará métricas específicas para ele, enquanto selecionar múltiplos canais comparará seu desempenho. Estas são as métricas disponíveis:

* [Contagem de Jobs de Importação](cs2-metrics.md#contagem-de-jobs-de-importacao)
* [Duração do Job de Importação](cs2-metrics.md#duracao-do-job-de-importacao)
* [Taxa de Falha do Job de Importação](cs2-metrics.md#taxa-de-falha-do-job-de-importacao)
* [Problemas no Job de Importação](cs2-metrics.md#problemas-no-job-de-importacao)
* [Bytes Processados no Job de Importação](cs2-metrics.md#taxa-de-falha-do-job-de-importacao)
* [Registros Processados no Job de Importação](cs2-metrics.md#registros-processados-no-job-de-importacao)
