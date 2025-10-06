A site for my ideas, projects, and activities. Built on the Jekyll Fresh theme.

## GitHub Pages Setup

This site is configured to deploy automatically to GitHub Pages using the custom domain `hugh-ferguson.com`.

### Configuration Files
- `_config.yml`: Jekyll configuration with proper baseurl and url settings
- `CNAME`: Custom domain configuration
- `.github/workflows/jekyll.yml`: GitHub Actions workflow for building and deploying the site
- `Gemfile`: Dependencies using the github-pages gem for compatibility

### To ensure the site works properly:

1. **GitHub Pages Settings**: In the repository settings, make sure:
   - Pages source is set to "GitHub Actions" 
   - Custom domain is set to `hugh-ferguson.com`
   - "Enforce HTTPS" is checked

2. **Domain Configuration**: The domain `hugh-ferguson.com` needs to be pointed to GitHub Pages:
   - Add DNS A records pointing to GitHub Pages IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Or add a CNAME record pointing to `hughferg.github.io`

3. **SSL Certificate**: GitHub will automatically provision an SSL certificate once the domain is properly configured

### Local Development

To run the site locally:
```bash
bundle install
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`
