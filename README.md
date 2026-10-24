Markdown
<div align="center">

# Compatra

### Prove your third-party APIs still work with your code.

Compatra ties every vendor API change to the code that calls it, then runs your own tests to see whether they would notice. Find out before your customers do.

[Website](https://compatra.com) · [Install GitHub App](#) · [Documentation](#)

---

</div>

## 🚀 Quick Start

Run a quick scan directly from your terminal—no setup or account required:

```bash
npx compatra scan
Note: The CLI runs locally on your machine. Nothing is uploaded.

✨ Features
Vendor API Mapping: Automatically ties third-party API changes and deprecations directly to the specific lines of code calling them.

Impact Testing: Runs your existing test suites against API updates to catch breaking changes before production.

Privacy-First Architecture: Local scans with zero code uploaded to external servers.

Continuous Integration: Seamlessly integrates with GitHub Actions and PR workflows.

💻 Usage
Quick Scan CLI
Bash
$ npx compatra scan

Vendor SDKs in this project:
  Stripe   stripe@^17.0.0

Checked against endpoints these vendors already deprecated:
  Stripe 6 deprecated
🛠️ GitHub Action Setup
Add Compatra to your repository workflow (.github/workflows/compatra.yml):

YAML
name: Compatra API Scan

on:
  push:
    branches: [ main ]
  pull_request:

jobs:
  scan:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Run Compatra Scan
        run: npx compatra scan
🌐 Connect with Us
🌐 Website: compatra.com

🔒 Security: Security Details & Privacy Policy

📝 Blog: Compatra Blog