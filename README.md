# Screen Porch Builder Website

Custom screened porch builder website for Upstate SC (Simpsonville, Fountain Inn, Gray Court & Laurens).

## Repository Structure

- `index.html` - Original version
- `screenporchbuilder-v2_1.html` - Version 2.1 with green theme
- `screenporchbuilder-v3.html` - Version 3 with dark theme (#1a1a1a base, #e07b25 orange CTAs)

## Auto-Deploy Setup

This repository is configured to automatically deploy to Hostinger when changes are pushed to the `main` branch.

### Setting Up GitHub Secrets

To enable auto-deployment, you need to add the following secrets to your GitHub repository:

1. Go to your GitHub repository: https://github.com/cscottburch1/screen-porch-builder
2. Click **Settings** > **Secrets and variables** > **Actions**
3. Click **New repository secret** and add each of the following:

#### Required Secrets:

- **FTP_SERVER**: Your Hostinger FTP server address
  - Example: `ftp.screenporchbuilder.com` or IP address like `123.456.789.012`
  - Find this in Hostinger Control Panel > **Files** > **FTP Accounts**

- **FTP_USERNAME**: Your FTP username
  - Find this in Hostinger Control Panel > **Files** > **FTP Accounts**
  - Usually something like `u123456789` or your domain

- **FTP_PASSWORD**: Your FTP password
  - This is the password you set when creating the FTP account
  - You can reset it in Hostinger Control Panel if needed

- **FTP_SERVER_DIR**: The directory path on your server
  - Usually `/public_html/` or `/public_html/screenporchbuilder.com/`
  - Some Hostinger accounts use `/domains/screenporchbuilder.com/public_html/`

### Finding Your Hostinger FTP Details

1. Log in to **Hostinger Control Panel** (hpanel.hostinger.com)
2. Navigate to **Files** > **FTP Accounts**
3. You'll see your FTP hostname, username, and port
4. If you don't have an FTP account, click **Create FTP Account**
5. The server directory is typically shown in the FTP account details

### Testing the Deployment

Once you've added all secrets:

1. Make a small change to any HTML file
2. Commit and push to the `main` branch:
   ```bash
   git add .
   git commit -m "Test deployment"
   git push
   ```
3. Go to your GitHub repository > **Actions** tab
4. Watch the deployment workflow run
5. Check your live site to confirm the changes

### Manual Deployment

You can also trigger a manual deployment:

1. Go to **Actions** tab in GitHub
2. Click **Deploy to Hostinger** workflow
3. Click **Run workflow** button
4. Select `main` branch and click **Run workflow**

## Local Development

Simply edit the HTML files and open them in your browser to preview changes. When ready to deploy, commit and push to GitHub.

## Support

For issues with:
- **GitHub Actions**: Check the Actions tab for error logs
- **FTP Connection**: Verify your Hostinger FTP credentials
- **Website Issues**: Check the HTML files for errors

---

**License**: SC #CLG118679  
**Contact**: (864) 724-4600 | estimates@burchcontracting.com
