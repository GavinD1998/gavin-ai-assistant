# Gavin AI Assistant — GitHub Pages site

This folder contains a static public information site for Gavin AI Assistant, an internal-use application for KEY Home Furnishings.

## Files

- `index.html` — home page
- `eula.html` — End-User License Agreement
- `privacy.html` — Privacy Policy
- `styles.css` — shared site styles

The site uses only HTML and CSS. It contains no JavaScript, application credentials, OAuth client IDs, client secrets, or access tokens.

## Publish with GitHub Pages

These steps use the GitHub website. GitHub CLI is not required.

### 1. Create a repository

1. Sign in at [github.com](https://github.com/).
2. Select the **+** menu in the upper-right corner, then select **New repository**.
3. In **Repository name**, enter `gavin-ai-assistant`.
4. Choose **Public**. GitHub Pages must be publicly reachable for service-provider production review.
5. Leave **Add a README file**, `.gitignore`, and license initialization unchecked because this folder already includes a README.
6. Select **Create repository**.

### 2. Upload the site files

1. On the new repository page, select **uploading an existing file**. If that link is not shown, select **Add file** and then **Upload files**.
2. Upload these five files from this folder: `index.html`, `eula.html`, `privacy.html`, `styles.css`, and `README.md`.
3. Confirm that the HTML and CSS files appear at the top level of the repository, not inside another folder.
4. In **Commit changes**, use a message such as `Add Gavin AI Assistant public pages`.
5. Commit directly to the `main` branch, then select **Commit changes**.

### 3. Enable GitHub Pages

1. Open the repository’s **Settings** tab.
2. In the left sidebar, select **Pages** under **Code and automation**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Under **Branch**, select `main`.
5. For the folder, select `/ (root)`.
6. Select **Save**.

GitHub will publish the site over HTTPS. The first deployment may take a few minutes. The Pages settings screen will show a message when the site is live.

### 4. Obtain the final HTTPS URLs

Replace `USERNAME` with the GitHub account or organization name that owns the repository:

- Home: `https://USERNAME.github.io/gavin-ai-assistant/`
- End-User License Agreement: `https://USERNAME.github.io/gavin-ai-assistant/eula.html`
- Privacy Policy: `https://USERNAME.github.io/gavin-ai-assistant/privacy.html`

The repository name is part of each URL. If a different repository name is used, replace `gavin-ai-assistant` in all three URLs.

### 5. Confirm public access

1. Sign out of GitHub or open a private/incognito browser window.
2. Open each of the three HTTPS URLs above.
3. Confirm that every page loads without a GitHub sign-in prompt.
4. On the home page, open both legal-document links and confirm they lead to the correct pages.
5. Confirm the browser shows an HTTPS connection.
6. Use the final EULA and Privacy Policy URLs in the corresponding Intuit production-app fields.

## Updating the site

Upload the revised file through **Add file** > **Upload files**, or edit the file directly on GitHub, and commit the change to `main`. GitHub Pages will deploy the update automatically. Review the effective date when changing either legal document.

## Before submitting to Intuit

- Verify the repository and all three pages are public.
- Verify the company name and contact email are correct.
- Verify the policy still matches the application’s actual data access, storage, processing, sharing, security, retention, and user controls.
- Never commit OAuth client IDs, client secrets, tokens, API keys, or other credentials.
