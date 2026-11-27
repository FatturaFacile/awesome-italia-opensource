# 🚀 Italia Open-Source

![Last Commit](https://img.shields.io/github/last-commit/italia-opensource/awesome-italia-opensource/main) 

The **only fully open-source platform** that transparently gives voice, discovers, and explores **Italy's tech innovations**.

Through a series of **awesome lists**, we seek to give visibility to open-source Projects, Communities, Tech blogs, Innovative startups, and more.

Feel free to make your contribution. If you want to add a new item to one or more lists please read the [contribution guidelines](https://github.com/italia-opensource/awesome-italia-opensource/blob/main/CONTRIBUTING.md) before opening a pull request or contributing to this repository

> **About this repository.** This is the FatturaFacile organization's fork of [italia-opensource/awesome-italia-opensource](https://github.com/italia-opensource/awesome-italia-opensource). It exists to list [FatturaFacile](https://github.com/FatturaFacile/FatturaFacile) among Italian open-source projects (`awesome/opensource/data/fattura-facile.json`) and is not part of the FatturaFacile product. The lists and tooling below come from the upstream project; contributions to the lists themselves belong upstream.

### 🟢 Website

[italiaopensource.com](https://italiaopensource.com)

### ☀️ Awesome Lists

- [List of Open-source projects](https://github.com/italia-opensource/awesome-italia-opensource/blob/main/awesome/opensource/README.md)

- [List of Tech Communities](https://github.com/italia-opensource/awesome-italia-opensource/blob/main/awesome/communities/README.md)

- [List of Digital Nomads](https://github.com/italia-opensource/awesome-italia-opensource/blob/main/awesome/digital-nomads/README.md)

- [List of Tech Startups](https://github.com/italia-opensource/awesome-italia-opensource/blob/main/awesome/startups/README.md)

### 📊 Analytics

In the [analytics/](analytics) folder, you will find all the aggregated data for each awesome list. This will allow you to access the data to download and use it most easily.

The aggregated file of open-source projects also contains statistical data and metadata retrieved via API from GitHub, allowing you to have a complete overview.

### 🛠 Local development

Requirements: Python 3.12 (see `.python-version`) and [uv](https://docs.astral.sh/uv/). Run `make` to list all targets.

```bash
make setup         # create the local environment and install pre-commit hooks
make lint          # pre-commit: gitleaks, ruff, ruff format, uv lock checks
make test          # validate the data against scheme/*.json and render the lists
make release       # check, build analytics and render (needs GitHub API access)
```

Repository layout: `awesome/<list>/data/*.json` (list entries), `scheme/` (JSON Schemas), `scripts/` (`check.py`, `process.py`, `render.py`), `analytics/` (aggregated data).

### 🔄 CI

- `Pull request` (`test.yml`): runs the data checks on pull requests to `main` that touch the lists, schemas or scripts.
- `Release` (`release.yml`): renders data, analytics and READMEs on pushes to `main`, monthly (15th) and on manual dispatch.
- Pull requests target `main` (this repository has no `dev` branch).

### 🔥 Our Contributors

<a href="https://github.com/italia-opensource/awesome-italia-opensource/graphs/contributors"> <img src="https://contrib.rocks/image?repo=italia-opensource/awesome-italia-opensource" /> </a>

### ❤️ Support us

<a href="https://opencollective.com/italia-open-source/donate" target="_blank">
  <img src="https://opencollective.com/italia-open-source/donate/button@2x.png?color=blue" width=200 />
</a>

### Join with us

[![LinkedIn](https://img.shields.io/badge/Linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/italia-open-source)

[![Telegram](https://img.shields.io/badge/Telegram-229ED9?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/+WsJ91uPMVbUzZjk0)

### License

The project is made available under the GPL-3.0 license. See the `LICENSE` file for more information.
