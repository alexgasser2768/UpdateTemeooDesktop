# Update

A brief documentation to Update TemeooDesktop Application


## Edit package.json

First edit the **DesktopApp/package.json** file

```json
"repository": {
  103      "type": "git",
  104      "url": "https://github.com/<username>/UpdateTemeooDesktop"
  105    },
```
and change the url fied to the corresponding repository

## Generate Token

[Generate Personal Access Token](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) for your Github account. Don't forget to select the scope "repo" when generating it.

## Deployment
When you want to deploy a new version of your code don't forget to change the version in the **/DesktopApp/release/app/package.json**



To deploy the project run

```bash
export GH_TOKEN=<YOUR_TOKEN> && npm run publish-win-package
```

## Repo

Once done go to the release section of the repository. A new release should appear.

To deploy the release move the the **Edit** section of the release and click on **publish release**.
## Support

For support, email alex.gasser@temeoo.fr.
