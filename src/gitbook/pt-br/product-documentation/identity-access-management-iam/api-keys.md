---
description: Learn more about API Keys and how to integrate them with our platform.
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

# Chaves de API

As Chaves de API permitem que você conceda acesso de uma API à sua conta BMS. Isso facilitará o acompanhamento de suas métricas usando uma plataforma externa. Algumas APIs, como o Zapier, podem ser configuradas para criar Anúncios com base em arquivos do Google Drive. Quando se trata de APIs, há muito que podemos fazer, e cada API terá suas particularidades. No entanto, a integração dessas APIs com o console da BMS é semelhante. Este artigo visa ajudá-lo a realizar essa integração.

## Gerenciando Chaves de API  <a href="#managing-api-keys" id="managing-api-keys"></a>

As Chaves de API estão disponíveis na página de permissões. Para acessá-la, clique no nome da sua conta no canto superior direito, depois clique em Permissões e, no menu à esquerda, clique em Chaves de API.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-10-08 092211.png" alt=""><figcaption><p>Lista de Chaves de API</p></figcaption></figure>

### Criando uma Chave de API <a href="#creating-an-api-key" id="creating-an-api-key"></a>

É possível [Criar Novas Chaves de API](api-keys.md#criar-nova-chave-de-api) e também [Vincular Chave de API Existente](api-keys.md#vincular-chave-de-api-existente).

#### Criar nova Chave de API

1. Clique em <img src="../../.gitbook/assets/image (106).png" alt="" data-size="line"> para adicionar uma Chave de API.
2.  Selecione Criar Chave de API e preencha as informações:

    <figure><img src="../../.gitbook/assets/Captura de tela 2024-10-08 100509.png" alt=""><figcaption><p>Editor de Chaves de API</p></figcaption></figure>



    * Nome: Defina um nome para sua Chave de API.
    * Tags: Defina tags para sua organização.
    * Políticas: Defina políticas de acesso que limitam a que esta Chave de API concede acesso. Clique em <img src="../../.gitbook/assets/image (108).png" alt="" data-size="original"> para adicionar suas políticas. Cada política tem um nome e uma descrição do acesso que ela concede. Você também pode criar a Chave de API sem selecionar uma política.

    <figure><img src="../../.gitbook/assets/image (978).png" alt=""><figcaption><p>Tela de Seleção de Políticas</p></figcaption></figure>

    * Após selecionar todas as políticas necessárias, clique em <img src="../../.gitbook/assets/image (1033).png" alt="" data-size="line"> para confirmar sua seleção.
3. Clique em <img src="../../.gitbook/assets/image (110).png" alt="" data-size="line"> para salvar sua Chave de API.

#### Vincular Chave de API Existente <a href="#link-existing-api-key" id="link-existing-api-key"></a>

Esta opção permite que você vincule uma Chave de API existente de outra conta BMS.

{% hint style="info" %}
Ao vincular uma Chave de API existente, você concederá acesso à sua conta para os usuários da Chave de API vinculada. Use políticas para controlar o que pode ser feito através desta Chave de API.
{% endhint %}

1. Clique em <img src="../../.gitbook/assets/image (106).png" alt="" data-size="line"> para adicionar uma Chave de API.
2.  Selecione **Vincular Chave de API existente** e preencha os detalhes:

    <figure><img src="../../.gitbook/assets/image (948).png" alt=""><figcaption><p>Vinculando uma API Existente</p></figcaption></figure>

    * ID da Chave de API: Informe o ID da Chave de API que você deseja vincular.
    * Políticas: Defina políticas de acesso que limitam o que esta Chave de API concede acesso, clicando em <img src="../../.gitbook/assets/image (108).png" alt="" data-size="original"> para adicionar suas políticas. Cada política requer um nome e uma descrição do acesso que fornece. Ao vincular Chaves de API, pelo menos uma política deve ser selecionada.
    * Após selecionar todas as políticas necessárias, clique em <img src="../../.gitbook/assets/image (1033).png" alt="" data-size="line"> para confirmar sua seleção.
3. Clique em <img src="../../.gitbook/assets/image (110).png" alt="" data-size="line"> para salvar sua Chave de API.

### Aba Códigos de Acesso <a href="#access-codes-tab" id="access-codes-tab"></a>

Após criar a Chave de API, você precisa gerar um Código de Acesso antes de poder começar a usá-la. Se você selecionar uma Chave de API vinculada, esta aba permanecerá desabilitada, pois não há necessidade de criar um código de acesso. Nesses casos, você usará o Código de Acesso da API vinculada, que pode ser fornecido por seu criador.

<figure><img src="../../.gitbook/assets/image (1035).png" alt=""><figcaption><p>Aba Códigos de Acesso</p></figcaption></figure>

1. Selecione a Chave de API para a qual o código de acesso precisa ser criado.
2.  Clique em <img src="../../.gitbook/assets/image (1036).png" alt="" data-size="line"> para criar um código de acesso para a Chave de API selecionada.\


    <figure><img src="../../.gitbook/assets/image (983).png" alt=""><figcaption><p>Aba Códigos de Acesso</p></figcaption></figure>
3. Insira uma descrição para seu código de acesso.
4. Clique em <img src="../../.gitbook/assets/image (1038).png" alt="" data-size="line"> para salvar seu código de acesso
5.  Logo após salvar suas alterações, o segredo do código de acesso será exibido assim:

    <figure><img src="../../.gitbook/assets/Captura de tela 2024-10-09 090427.png" alt=""><figcaption><p>Segredo do Código de Acesso</p></figcaption></figure>
6. É possível copiar o segredo usando o botão de copiar, <img src="../../.gitbook/assets/image (1039).png" alt="" data-size="original">, ou baixá-lo em um arquivo .txt.

Você pode criar até 2 códigos de acesso por Chave de API. Cada código é válido por 365 dias. Aconselhamos fortemente que você crie um novo código algumas semanas antes que o código atual expire para garantir que os serviços que dependem desta Chave de API não parem.

### Como Acessar a BMS via API <a href="#how-to-access-bms-via-api" id="how-to-access-bms-via-api"></a>

Para interagir com os serviços da BMS programaticamente, você precisa incluir o Código de Acesso gerado em suas requisições de API. Seu acesso será restrito às APIs específicas que sua chave de API está autorizada a usar. Você pode incluir o Código de Acesso em suas requisições usando um dos seguintes métodos:

*   **No Cabeçalho da Requisição:** Copie o valor para o cabeçalho `x-api-key`. Para isso, use o botão <img src="../../.gitbook/assets/image (985).png" alt="" data-size="original">. Isso evitará erros de digitação. Cole-o no cabeçalho de suas requisições.

    <figure><img src="../../.gitbook/assets/image (984).png" alt=""><figcaption><p>Acessando a BMS via API - Método via Cabeçalho da Requisição</p></figcaption></figure>
*   **Na Query String:** Adicione o Código de Acesso à URL como um parâmetro de consulta apiKey. Você também pode usar o botão de copiar para evitar erros de digitação.

    <figure><img src="../../.gitbook/assets/image (986).png" alt=""><figcaption><p>Acessando a BMS via API -Método Query String</p></figcaption></figure>

Para uma lista completa das APIs da BMS disponíveis, por favor, consulte nossa [documentação](https://api.bluems.com/).

### **Editando Chaves de API e Códigos de Acesso** <a href="#editing-api-keys-and-access-codes" id="editing-api-keys-and-access-codes"></a>

Todos os detalhes das Chaves de API estão disponíveis para edição clicando em <img src="../../.gitbook/assets/image (1040).png" alt="" data-size="line"> na mesma linha da Chave de API que você deseja editar. Após fazer suas alterações, clique em <img src="../../.gitbook/assets/image (1041).png" alt="" data-size="line"> para salvá-las.&#x20;

Você também pode excluir uma Chave de API clicando em <img src="../../.gitbook/assets/image (1042).png" alt="" data-size="original">, e, em seguida, confirmando a ação em<img src="../../.gitbook/assets/image (1043).png" alt="" data-size="line">. Tenha cuidado - esta ação não pode ser desfeita. Lembre-se de que qualquer API que dependa da Chave de API excluída deixará de funcionar.\
\
Em relação aos Códigos de Acesso, você pode visualizar o segredo e baixar as credenciais clicando em <img src="../../.gitbook/assets/image (1044).png" alt="" data-size="original">na mesma linha do código de acesso. A descrição do código de acesso também pode ser editada clicando em <img src="../../.gitbook/assets/image (1040).png" alt="" data-size="line">. Quando terminar, clique em <img src="../../.gitbook/assets/image (1041).png" alt="" data-size="line"> para salvar suas mudanças.

{% hint style="danger" %}
Atenção! Tenha cuidado ao excluir um código de acesso. Esta ação não pode ser desfeita, e todos os serviços que dependem deste código de acesso deixarão de funcionar.
{% endhint %}

Você também pode excluir códigos de acesso. Isso é útil em casos onde os dados possam ter sido comprometidos. Para fazer isso, primeiro desabilite o código movendo a chave seletora para a posição de desligado <img src="../../.gitbook/assets/image (1045).png" alt="" data-size="original"> e, em seguida, clicando em <img src="../../.gitbook/assets/image (1042).png" alt="" data-size="original"> na mesma linha do código de acesso que deseja excluir e confirmando em <img src="../../.gitbook/assets/image (1043).png" alt="" data-size="line">.&#x20;
