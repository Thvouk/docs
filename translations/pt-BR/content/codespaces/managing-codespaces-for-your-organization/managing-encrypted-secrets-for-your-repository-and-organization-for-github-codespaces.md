---
title: Managing encrypted secrets for your repository and organization for GitHub Codespaces
shortTitle: Segredos criptografados
intro: 'Os segredos criptografados permitem que você armazene informações confidenciais na sua organização, repositório ou {% data variables.product.prodname_github_codespaces %}.'
product: '{% data reusables.gated-features.codespaces %}'
permissions: 'To manage secrets for {% data variables.product.prodname_github_codespaces %} for an organization, you must be an organization owner.'
versions:
  fpt: '*'
  ghec: '*'
topics:
  - Codespaces
  - Secret store
  - Security
redirect_from:
  - /codespaces/managing-codespaces-for-your-organization/managing-encrypted-secrets-for-your-repository-and-organization-for-codespaces
---

 

## Sobre segredos

Segredos são variáveis de ambiente criptografadas que você cria em uma organização ou repositório. Os segredos que você criou estão disponíveis para uso em {% data variables.product.prodname_github_codespaces %}. O GitHub usa uma [caixa protegida pela libsodium](https://libsodium.gitbook.io/doc/public-key_cryptography/sealed_boxes) para criptografar segredos antes que eles cheguem ao GitHub e só descriptografa quando você os usa em um codespace.

Os segredos no nível da organização permitem que você compartilhe segredos entre vários repositórios, o que reduz a necessidade de criar segredos duplicados. Você pode usar políticas de acesso para controlar quais repositórios podem usar segredos da organização.

{% data reusables.codespaces.secrets-on-start %}

### Nomeando segredos

{% data reusables.codespaces.secrets-naming %} Por exemplo, um segredo criado no nível do repositório deve ter um nome exclusivo nesse repositório, e um segredo criado no nível da organização deve ter um nome exclusivo nesse nível.

  {% data reusables.codespaces.secret-precedence %}

### Limites para segredos

Você pode armazenar até 100 segredos por organização e 100 segredos por repositório.

Os segredos são limitados a 64 kB.

## Adicionar segredos para um repositório

Para criar segredos para um repositório da organização, você deve ter acesso de administrador.

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-settings %}
1. Na seção "Segurança" da barra lateral, selecione **Segredos de {% octicon "key-asterisk" aria-label="The key-asterisk icon" %}** e, em seguida, clique em **{% data variables.product.prodname_codespaces %}**.
2. Na parte superior da página, clique em **Novo segredo de repositório**.
3. Digite um nome para o seu segredo na caixa de entrada **Nome**.
4. Insira o valor para o seu segredo.
5. Clique em **Add secret** (Adicionar segredo).

## Adicionar segredos para uma organização

Ao criar um segredo em uma organização, você pode usar uma política para limitar quais repositórios podem acessar esse segredo. Por exemplo, você pode conceder acesso a todos os repositórios ou limitar o acesso a apenas repositórios privados ou a uma lista específica de repositórios.

{% data reusables.actions.permissions-statement-secrets-organization %}

{% data reusables.organizations.navigate-to-org %}
{% data reusables.organizations.org_settings %}
1. Na seção "Segurança" da barra lateral, selecione **Segredos de {% octicon "key-asterisk" aria-label="The key-asterisk icon" %}** e, em seguida, clique em **{% data variables.product.prodname_codespaces %}**.
2. Na parte superior da página, clique em **Novo segredo de organização**.
3. Digite um nome para o seu segredo na caixa de entrada **Nome**.
4. Insira o **Valor** para o seu segredo.
5. Na lista suspensa **Acesso do repositório**, escolha uma política de acesso. ![Lista de Acesso ao Repositório com repositórios privados selecionados](/assets/images/help/codespaces/secret-repository-access.png)
6. Clique em **Add secret** (Adicionar segredo).

## Rever o acesso para os segredos do nível da organização

Você pode verificar quais políticas de acesso são aplicadas a um segredo na sua organização.

{% data reusables.organizations.navigate-to-org %}
{% data reusables.organizations.org_settings %}
{% data reusables.actions.sidebar-secret %}
1. A lista de segredos inclui quaisquer permissões e políticas configuradas. Por exemplo: ![Lista de segredos](/assets/images/help/settings/actions-org-secrets-list.png)
1. Para obter mais detalhes sobre as permissões configuradas para cada segredo, clique em **Atualizar**.

## Leia mais

- "[Gerenciar segredos criptografados nos seus codespaces](/codespaces/managing-your-codespaces/managing-encrypted-secrets-for-your-codespaces)"
