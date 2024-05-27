[![Update Resume Gist](https://github.com/mapleDevJS/resume/actions/workflows/gist.yml/badge.svg)](https://github.com/mapleDevJS/resume/actions/workflows/gist.yml)

Hosting your resume becomes incredibly simple by leveraging `resume.json` on gist.github.com. For instance, have a look at mine hosted at https://gist.github.com/mapleDevJS/3c39460fb5a68950bc8899fe846fe81f. Now it's automatically accessible at https://registry.jsonresume.org/mapleDevJS. Editing your Gist via the online GUI is hassle-free and ensures updates within no time, typically less than a minute!

## Advanced Usage
In case you prefer a repository-based approach for your `resume.json`—similar to this sample, you can set up a Github Action for automatic gist updates with the latest `resume.json` from your repo whenever you push.

Here's how you can do it:

1) Create a new gist and name it `resume.json`.
2) Either create or fork this repo and commit your updated `resume.json`.
3) Generate a Personal Github token (with 'gist' scope only) to authorize necessary actions.
4) Navigate to your repository settings, find the secrets page, and add a new secret named `TOKEN`. Use the token you created in step 3 as its value.
5) Now just push to your repo. This will update your gist's `resume.json` to match the one in your repository, hence updating the registry.

Don't forget to check the `.github/workflows/gist.yml` file to understand how things work in detail. If you need any assistance, feel free to open an issue. Enjoy your seamless and automated `resume.json` hosting experience!