# Azure AD B2C custom page UI templates

AzureBlue custom page UI templates for Azure AD B2C user flows.

## Templates

- `templates/AzureBlue/unified.html`
- `templates/AzureBlue/selfAsserted.html`
- `templates/AzureBlue/exception.html`

The templates start from the AzureBlue tenant templates. The self-asserted template hides the built-in `Cancel` action, which avoids the buggy cancel behavior in forgot-password and change-password journeys.

Upload the files to a publicly accessible host and configure the user flow's **Page layout** / **Custom page URI** settings to reference the appropriate file. Use the `.html` files when hosting on GitHub Pages: they are served as `text/html`, whereas `.cshtml` files are served as a generic binary type.

These templates reference Azure-hosted AzureBlue assets, so they do not currently include a local copy of the CSS, fonts, images, or JavaScript assets.
