# devopsPracticeAzure
  ## azure_login.yml
    1. Create a Subscription
    2. Create a Service Principal
    3. Assign a role for this SP in subscripton
    4. Create federated credential OIDC connection for entity type: environment or branch
    5. if its an environment create an environment(Settings → Environments) say "dev" and below values in environment-dev-variables
    6.  update code
          client-id: ${{ vars.AZURE_CLIENT_ID }}
          tenant-id: ${{ vars.AZURE_TENANT_ID }}
          subscription-id: ${{ vars.AZURE_SUBSCRIPTION_ID }}
