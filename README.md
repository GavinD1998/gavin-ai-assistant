# Gavin AI Assistant — GitHub Pages site

This folder contains a static public information site for Gavin AI Assistant, an internal-use application for KEY Home Furnishings.

## Files

- `index.html` — home page
- `eula.html` — End-User License Agreement
- `privacy.html` — Privacy Policy
- `security.html` — Security practices
- `quickbooks-callback.html` — static QuickBooks Production OAuth callback page
- `styles.css` — shared site styles

The public information pages use only HTML and CSS. The QuickBooks callback page contains a small inline script that reads the current browser URL and copies it to the clipboard. It does not exchange authorization codes, call Intuit token endpoints, persist OAuth values, or transmit them to another service. The site contains no application credentials, OAuth client IDs, client secrets, access tokens, or refresh tokens.

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
2. Upload these six files from this folder: `index.html`, `eula.html`, `privacy.html`, `security.html`, `styles.css`, and `README.md`.
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
- Security: `https://USERNAME.github.io/gavin-ai-assistant/security.html`

For the expected GitHub account, the Security page URL is:

`https://gavind1998.github.io/gavin-ai-assistant/security.html`

The repository name is part of each URL. If a different repository name is used, replace `gavin-ai-assistant` in all four URLs.

### 5. Confirm public access

1. Sign out of GitHub or open a private/incognito browser window.
2. Open each of the four HTTPS URLs above.
3. Confirm that every page loads without a GitHub sign-in prompt.
4. On the home page, open the EULA, Privacy Policy, and Security links and confirm they lead to the correct pages.
5. On every page, confirm the Security link appears in both the navigation and footer and opens `security.html`.
6. Confirm the browser shows an HTTPS connection.
7. Use the final EULA, Privacy Policy, and Security URLs in the corresponding Intuit production-app fields where requested.

## Updating the site

Upload the revised file through **Add file** > **Upload files**, or edit the file directly on GitHub, and commit the change to `main`. GitHub Pages will deploy the update automatically. Review the effective date when changing either legal document.

## Production QuickBooks OAuth

Exact Intuit Production Redirect URI:

`https://gavind1998.github.io/gavin-ai-assistant/quickbooks-callback.html`

The redirect URI registered with Intuit and the redirect URI saved in Gavin AI Assistant must match exactly. Every character matters, including `https`, the hostname, repository path, filename, capitalization, and trailing-slash behavior. The registered URI has no trailing slash.

### Publish and verify the callback

1. Upload `quickbooks-callback.html`, the updated `styles.css`, the updated `README.md`, and any other updated site files.
2. Commit the changes to the branch used by GitHub Pages.
3. Wait for the GitHub Pages deployment to finish.
4. Open `https://gavind1998.github.io/gavin-ai-assistant/quickbooks-callback.html` directly and confirm the informational state loads.
5. Confirm the page loads over HTTPS.
6. Confirm the **Copy Complete Callback URL** button is not shown when the page is opened without OAuth parameters.
7. Register the exact URI in **Intuit Developer → Gavin AI Assistant → Settings → Redirect URIs → Production**.
8. Enter the exact same URI in **Gavin AI Assistant → Settings → QuickBooks → Production → Registered Production Redirect URI**.

For a non-secret functional check, append dummy `code`, `state`, and `realmId` values to the URL. Confirm the success state appears and **Copy Complete Callback URL** copies the entire browser URL exactly. Do not use real OAuth values for this publishing check.

GitHub Pages controls HTTP response headers and does not provide repository-level configuration for custom `Cache-Control` headers. The callback page includes best-effort HTML cache directives, does not persist its URL in browser storage or cookies, and does not forward query values in page code. The initial HTTPS request necessarily reaches GitHub Pages at the callback URL. OAuth values may also remain in normal browser history until the user closes or clears it.

## Before submitting to Intuit

- Verify the repository and all four pages are public.
- Verify the company name and contact email are correct.
- Verify the policy still matches the application’s actual data access, storage, processing, sharing, security, retention, and user controls.
- Never commit OAuth client IDs, client secrets, tokens, API keys, or other credentials.
2. Open each of the four HTTPS URLs above.
3. Confirm that every page loads without a GitHub sign-in prompt.
4. On the home page, open the EULA, Privacy Policy, and Security links and confirm they lead to the correct pages.
5. On every page, confirm the Security link appears in both the navigation and footer and opens `security.html`.
6. Confirm the browser shows an HTTPS connection.
7. Use the final EULA, Privacy Policy, and Security URLs in the corresponding Intuit production-app fields where requested.

## Updating the site

Upload the revised file through **Add file** > **Upload files**, or edit the file directly on GitHub, and commit the change to `main`. GitHub Pages will deploy the update automatically. Review the effective date when changing either legal document.

## Before submitting to Intuit

- Verify the repository and all four pages are public.
- Verify the company name and contact email are correct.
- Verify the policy still matches the application’s actual data access, storage, processing, sharing, security, retention, and user controls.
- Never commit OAuth client IDs, client secrets, tokens, API keys, or other credentials.
