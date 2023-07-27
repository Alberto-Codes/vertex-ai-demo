# Development Environment

To open this project in Codespaces:

1. Fork this repository to your GitHub account.

2. On your forked repository page, click the "Code" button:

![Code button](docs/images/code_button.png)

3. Select "Open with Codespaces" from the dropdown.

4. When prompted, create the codespace on the `development` branch. 

This will:

- Create a cloud dev environment. 

- Install dependencies.

- Connect the forked GitHub repo.

- Install VSCode extensions

You can now run scripts and notebooks in the Codespaces IDE.

## Connect to Google Cloud Platform

### Authentication
You will need to authenticate from Github Codespaces to the Google Cloud Platform using the installed Google Cloud CLI SDK.  The following commant will iniate the login flow to authenticate with your GCP account.
```bash
gcloud auth login
```
This will open a browser window prompting you to login and authorize account access.

Login with your Google account.

Click Allow on the consent screen.

Copy the authorization code.

Back in Codespaces, paste the copied authorization code at the prompt to complete login.

### Create GCP Project
You only need to do this once.  If you haven't created a project skip down to Switch to Project section
```bash
gcloud projects create vertex-ai-gcp-demo
```

### Check Project
```bash
gcloud projects describe vertex-ai-gcp-demo
```

### Switch to Project
```bash
gcloud config set project vertex-ai-gcp-demo
```
