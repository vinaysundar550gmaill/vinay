Você precisa de um token de acesso para publicar, instalar e excluir pacotes no {{ site.data.variables.product.prodname_registry }}. Você pode usar um token de acesso pessoal para autenticar com seu nome de usuário diretamente no {% data variables.product.prodname_registry %} ou na API {% data variables.product.prodname_dotcom %}. Ao criar um token de acesso pessoal, você pode atribuir diferentes escopos de token, dependendo da sua necessidade.

{% if currentVersion == "free-pro-team@latest" %}
Para efetuar a autenticação usando um
fluxo de trabalho do {% data variables.product.prodname_actions %}:
- Para registros de pacotes (`PACKAGE-REGISTRY.pkg.github.com`), você pode usar um `GITHUB_TOKEN`.
- For the container registry (`ghcr.io/OWNER/IMAGE-NAME`), you can use a `GITHUB_TOKEN` or a personal access token. We strongly recommend you use a `GITHUB_TOKEN` to avoid unncessary access to your repositories.

For more information about `GITHUB_TOKEN` used in {% data variables.product.prodname_actions %} workflows, see "[Encrypted secrets](/actions/reference/encrypted-secrets)" and "[Authentication in a workflow](/actions/reference/authentication-in-a-workflow#using-the-github_token-in-a-workflow)."

{% else %}
Para efetuar a autenticação em
{% data variables.product.prodname_registry %} usando um fluxo de trabalho de {% data variables.product.prodname_actions %}, você deve usar `GITHUB_TOKEN`.
{% endif %}
