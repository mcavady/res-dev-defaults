# res-dev-defaults - Shopify CLI3+ - CI__scss__WIP
Default setup for Shopify With CI workflow - scss and task running for css

<h1> You will need </h1>
<p> --- Github Applications --- </p>
<ul>
<li>Lighthouse CI</li>
<li>Shopify</li>
</ul>

<p> --- Workflow SECRET KEYS for actions to work --- </p>
<ul>
<li> LHCI_GITHUB_APP_TOKEN - from lighthouse github app </li>
<li> SHOP_ACCESS_TOKEN - from Shopify dashboard </li>
<li> SHOP_STORE - shopify store URL WHITOUT "https://" and WITHOUT "trailing slash" eg store-name.myshopify.com </li>
<li> SHOP_STORE_PASS - the store password ( password protected store )</li>
<li> SLACK_WEBHOOK - you will need to get this from your slack admin panel </li>
<li> <strong>YOU WILL NEED THE SHOPIFY TEST PRODUCTS FOR CI IN YOUR STORE FOR THIS TO WORK!</strong> the CI expects certain URLS to be present for testing</li>
</ul>

<p> --- optional Code security and analysis --- </p>
<ul>
<li>Dependabot - enable via GIT settings </li>
</ul>

<h1>Usage</h1>
--- install deps ---
<ul>
<li>run npm install from root folder</li>
<li>update deps if required</li>

</ul>

--- running in cli3 ---
<ul>
<li>login to dev store with CLI3 ( turn of hot reload optional flag ) upto you :)</li>
<li>run gulpfile</li>
</ul>

<h1>Notes</h1>
<ul>
<li>The task runner will compile css to assets folder</li>
<li>Shopify will ignore anything outside off the folder structure it expects</li>
<li>Dependabot can be set to auto update deps and the CI will check for a merge or push to "main" by default ( you can change this in the .github/workflows/main.yml</li>
</ul>

