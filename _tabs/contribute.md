---
# layout: archives
icon: fas fa-pen
order: 2
---

> If you know of an MPC deployment that has been **deployed** and reached a **substantial number of users** in practice, submit a PR to add a deployment. Or update an existing entry!
{: .prompt-tip }

To add a new MPC deployment, you simply need to create a PR with a new Markdown file.
1. Add yourself as an author in [`/_data/authors.yml`](https://github.com/dots-platform/dots-platform.github.io/blob/master/_data/authors.yml). The first element will be your author ID and the first link will be where on the web people can find you.
2. Copy the [`/_posts/YYYY-MM-DD-Title.md`](https://github.com/dots-platform/dots-platform.github.io/blob/master/_posts/YYYY-MM-DD-Title.md) template file in the [`/_posts/`](https://github.com/dots-platform/dots-platform.github.io/tree/main/_posts) directory.
3. Fill in the deployment's information. Details above the `---` and the description are required. For examples of what text and typography is supported, see these [template](https://chirpy.cotes.page/posts/text-and-typography/) [resources](https://github.com/cotes2020/jekyll-theme-chirpy/blob/master/_posts/2019-08-08-text-and-typography.md). Posts should be concise technical summaries with an emphasis on links to where readers can learn more. Refrain from "advertising" the deployment; keep it informational.
4. Submit the PR with a description of the change to [github.com/dots-platform/dots-platform.github.io](https://github.com/dots-platform/dots-platform.github.io). To help us out, please [confirm locally](https://chirpy.cotes.page/posts/getting-started/#running-local-server) that your version renders. Include how many users the deployment has reached.
5. We will review the PR, suggest any changes, and hopefully merge your update!
