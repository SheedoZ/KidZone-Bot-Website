# KidZone Bot information pages

Public Arabic and English privacy policy and data deletion instructions for KidZone Bot.

- Intended site: https://kidzone.premiumpower-eg.com/
- Privacy policy: https://kidzone.premiumpower-eg.com/privacy/
- Data deletion instructions: https://kidzone.premiumpower-eg.com/data-deletion/
- Operator: Mohamed Hashad

## Hosting

This is an independent static GitHub Pages site. Publish the root of `main`.
Configure the custom domain before adding the DNS record.

DNS at GoDaddy: add `CNAME`, name `kidzone`, value `SheedoZ.github.io`.
Keep existing Premium Power records and website settings unchanged.
Enable HTTPS when GitHub's certificate is ready.

## Files and checks

`index.html` links to the two policies. `policies.css` is shared styling.
No JavaScript, forms, tracking scripts or third-party page assets are included.

Run `git diff --check`, then `python -m http.server 8080 --bind 127.0.0.1`.
Check `/`, `/privacy/`, `/data-deletion/`, links and mobile layout.
Stop the local server after verification. Policy text changes must reflect the actual bot workflow.
Never commit credentials, runtime records or private product files here.

## Rollback

Revert the policy-page merge commit through a reviewed PR, then verify Pages.
If retiring the site, remove the `kidzone` DNS record before disabling Pages or removing its custom domain.
Do not alter the `www`, apex or other subdomain records of Premium Power.