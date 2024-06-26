{% ifversion fpt %}
1. Navigate to the main page of the repository or organization where your self-hosted runner groups are located.
2. Clique em {% octicon "gear" aria-label="The Settings gear" %} **Configurações**.
3. Na barra lateral esquerda, clique em **Actions** (Ações).
4. Click **Runner groups**.
{% elsif ghec or ghes or ghae %}
1. Navigate to where your self-hosted runner groups are located:
   * **In an organization**: navigate to the main page and click {% octicon "gear" aria-label="The Settings gear" %} **Settings**.{% ifversion ghec %}
   * **If using an enterprise account**: navigate to your enterprise account by clicking your profile photo in the top-right corner of {% data variables.product.prodname_dotcom_the_website %}, then clicking **Your enterprises**, then clicking the enterprise.{% elsif ghes or ghae %}
   * **Se estiver usando um executor de nível corporativo**:
     1. No canto superior direito de qualquer página, clique em {% octicon "rocket" aria-label="The rocket ship" %}.
     2. Na barra lateral esquerda, clique em **Visão geral da empresa**.
     3. In the enterprise sidebar, click {% octicon "law" aria-label="The law icon" %} **Policies**.{% endif %}
2. Navigate to the "Runner groups" settings:
   * **In an organization**: Click **Actions** in the left sidebar, then click {% ifversion fpt or ghec or ghes > 3.3 or ghae-issue-5091 %}**Runner groups**{% elsif ghae or ghes < 3.4 %}**Runners**{% endif %} below it.{% ifversion ghec or ghes or ghae %}
   * {% ifversion ghec %}**If using an enterprise account**:{% elsif ghes or ghae %}**If using an enterprise-level runner**:{% endif %} Click **Actions** under "{% octicon "law" aria-label="The law icon" %} Policies", then click the {% ifversion ghec or ghes > 3.3 or ghae-issue-5091 %}**Runners groups**{% elsif ghae or ghes < 3.4 %}**Runners**{% endif %} tab.{% endif %}
{% endif %}
