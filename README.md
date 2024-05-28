## Update Resume Gist

[![Update Resume Gist](https://github.com/mapleDevJS/resume/actions/workflows/gist.yml/badge.svg)](https://github.com/mapleDevJS/resume/actions/workflows/gist.yml)

This guide explains how to host your resume on `gist.github.com` using `resume.json`. See my hosted resume as an example at [https://gist.github.com/mapleDevJS/3c39460fb5a68950bc8899fe846fe81f](https://gist.github.com/mapleDevJS/3c39460fb5a68950bc8899fe846fe81f).

**Key Benefits:**
- Your resume becomes automatically accessible at [https://registry.jsonresume.org/mapleDevJS](https://registry.jsonresume.org/mapleDevJS).
- Updating your Gist via the online GUI is quick and hassle-free.

## Advanced Usage

For those who prefer a repository-based approach for `resume.json`, automatic gist updates can be set up with a Github Action. Whenever you push, your gist gets updated with the latest `resume.json` from your repository.

Here are the steps:

1) Create a new gist and name it `resume.json`.
2) Create or fork this repo and commit your updated `resume.json`.
3) Generate a Personal Github token (with the 'gist' scope only) for authorization.
4) Navigate to your repository settings, go to the secrets page, and add a new secret named `TOKEN`. Use the token you created in step 3 as the value.
5) Push to your repo. This updates your gist's `resume.json` to match the one in your repository, and consequently updates the registry.

Refer to the `.github/workflows/gist.yml` file for a detailed understanding. If you need assistance, feel free to open an issue.

Enjoy seamless, automated hosting of your `resume.json`!