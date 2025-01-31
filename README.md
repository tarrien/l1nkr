# l1nkr

Please follow the instructions below to finish the setup of your new L1nkr site.

## Installation

1) Add a LICENSE to your repo.
2) Clone your version of the template to your local computer:
```shell
git clone https://github.com/tarrien/l1nkr
```
3) Modify `config/_default/hugo.yaml` and `config/_default/params.yaml` according to your needs. Find more info on the theme [wiki](https://github.com/chrede88/L1nkr/wiki/Configuration).
4) Build a local version of your site by executing `hugo server` at the root of the repository. You can see the site by navigating to `http://localhost:1313/l1nkr/` (actual URL will be outputted in the CLI) in a browser.

---

## Configuration

See the [wiki](https://github.com/chrede88/L1nkr/wiki) for all info about configuration.

---

## Update the Theme Version

The theme version used to build the site is defined in `go.mod` file.

The best practice is to update to released and tested versions. To update to a specific version execute the following command in a terminal/commandline (at the root path of your site repo):

```shell
  hugo mod get github.com/chrede88/L1nkr@vX.Y.Z
```
Replace X,Y & Z with the corresponding version numbers. You can find the releases [here](https://github.com/chrede88/L1nkr/releases). Please check if any breaking changes are listed under the release you want to update to, before proceeding.

---

## Deploy on Github Pages
You can very easily deploy your site using Github Pages. Included in this template is a Github Action workflow that will build and deploy your site to Github Pages automatically:+1:

You can find the workflow here `.github/deploymentWorkflow/buildDeploy.yml`. To use this, move it to `.github/workflows/`.

The workflow is already set up and ready to go, but go through it and spend some time to understand what's going on. Otherwise, it'll always be this black box of magic that you can't fix when it breaks!

Last step: Go to Settings -> Pages -> Build and deployment -> Set the Source to "Github Actions".

Next time you publish a release this workflow will build and deploy your site :tada:

Your site will be published to the following URL:
`https://tarrien.github.io/l1nkr`