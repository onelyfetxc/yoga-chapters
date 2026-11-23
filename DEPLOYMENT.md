# GitHub Pages and domain setup

The repository includes a `CNAME` file for `theyogachapters.com`.

## Enable GitHub Pages

1. Open the repository on GitHub and go to **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select the `main` branch and the `/ (root)` folder, then save.
4. Under **Custom domain**, enter `theyogachapters.com` and save.

## Add DNS records

At the company where `theyogachapters.com` is registered, remove any conflicting records for `@` or `www`, then add:

| Type | Host | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | onelyfetxc.github.io |

Do not add a wildcard (`*`) DNS record.

## Finish

1. Wait for GitHub's DNS check to succeed. DNS updates can take time to propagate.
2. In **Settings → Pages**, turn on **Enforce HTTPS** when the checkbox becomes available.
3. Test both `https://theyogachapters.com` and `https://www.theyogachapters.com`.
