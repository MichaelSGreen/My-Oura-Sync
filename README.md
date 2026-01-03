# My Oura Sync - Legal Documentation

This repository contains the legal documentation pages required for the My Oura Sync OAuth application. These pages are hosted via GitHub Pages and linked in the Oura OAuth app registration.

## What's Included

- **index.html** - Landing page with links to legal documents
- **privacy.html** - Complete Privacy Policy
- **terms.html** - Complete Terms of Service
- **styles.css** - Shared responsive styling
- **.gitignore** - Basic web project exclusions

## Setting Up GitHub Pages

Follow these steps to publish your legal pages:

### 1. Create the Repository

If you haven't already:
```bash
git clone https://github.com/<your-username>/My-Oura-Sync.git
cd My-Oura-Sync
git add .
git commit -m "Add legal documentation pages"
git push
```

### 2. Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/<your-username>/My-Oura-Sync`
2. Click **Settings** (in the repository menu)
3. Scroll down and click **Pages** (in the left sidebar)
4. Under **Source**, select:
   - **Deploy from a branch**
   - Branch: **main** (or **master** if that's your default branch)
   - Folder: **/ (root)**
5. Click **Save**

GitHub will build and deploy your site. This typically takes 1-2 minutes.

### 3. Verify Deployment

Once deployed, your pages will be available at:

```
https://<your-username>.github.io/My-Oura-Sync/
```

**Important:** Test both legal pages in an incognito/private browser window to ensure they're publicly accessible:
- Privacy Policy: `https://<your-username>.github.io/My-Oura-Sync/privacy.html`
- Terms of Service: `https://<your-username>.github.io/My-Oura-Sync/terms.html`

## URLs for Oura OAuth App Form

When registering your OAuth application with Oura, use these URLs:

**Privacy Policy URL:**
```
https://<your-username>.github.io/My-Oura-Sync/privacy.html
```

**Terms of Service URL:**
```
https://<your-username>.github.io/My-Oura-Sync/terms.html
```

Replace `<your-username>` with your actual GitHub username.

## Pre-Launch Checklist

Before submitting your Oura OAuth application:

- [ ] **Pages are live**: Confirm both privacy.html and terms.html load in an incognito browser window
- [ ] **URLs are correct**: The URLs you paste into the Oura app form exactly match your deployed pages
- [ ] **Redirect URI matches**: Your redirect URI(s) in the Oura app form match your actual callback URL(s) (localhost for development, your production domain for production)
- [ ] **Review data scopes**: Confirm the "data types accessed" wording in privacy.html matches the OAuth scopes you're actually requesting from Oura
- [ ] **Contact email works**: Test that prometheusfoundation@gmail.com is monitored and responsive

## Customization (Optional)

### Update Data Types

If you're requesting different OAuth scopes than listed, update the data types section in `privacy.html`:

```html
<ul>
    <li>Sleep data and metrics</li>
    <li>Readiness scores and related metrics</li>
    <!-- Add or remove items to match your scopes -->
</ul>
```

### Branding and Styling

- Modify `styles.css` to adjust colors, fonts, or layout
- All pages share the same stylesheet for consistency
- The design is responsive and mobile-friendly

## Contact

For questions about this project or the My Oura Sync application:

**Email:** prometheusfoundation@gmail.com

## License

These legal documents are specific to the My Oura Sync application. Please do not reuse them verbatim for other projects - consult with legal counsel for your own terms and privacy policy.