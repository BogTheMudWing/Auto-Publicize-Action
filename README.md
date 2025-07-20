# Auto-Publicize-Action
A GitHub action that makes a repository public after six months of inactivity. I created this project to publish my personal knowledge base in the unusual event that I would not update it for six months.

## Quick Start
1. Go to https://github.com/settings/tokens?type=beta and create a new Personal Access Token.
2. Give the token a name and set the expiration to a custom date. This token will only be used for this action, so set it to the latest possible date. Keep in mind that at any given time this token must not expire within six months.
3. Set the repository access to "Only select repositories" and select the repo(s) you want to auto-publicize.
4. Under the "Repository Permissions" dropdown, set _Administration_ to _Read and Write_.
5. Generate the token and copy it to your clipboard.
6. Go to your repo settings and open the _Actions Secrets_ page (https://github.com/OWNER/REPO/settings/secrets/actions)
7. Create a new repo secret titled **TOKEN** and paste in the token, then save.
8. Go to the Actions tab (https://github.com/OWNER/REPO/actions) and create a new workflow.
9. Copy and paste the entire contents of [auto-publicize.yml](auto-publicize.yml)

That's it! Make sure to create a reminder to regenerate your token and update the secret six months before it expires. If you have any questions, please [create an issue](https://github.com/Stonley890/Auto-Publicize-Action/issues/new).

---

[![Bog The MudWing](https://blog.macver.org/content/images/2025/07/Stamp-Colored-Small-Shadow.png)](https://blog.macver.org/about-me)
