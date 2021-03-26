# goerz.github.io

This repository serves the static website at https://goerz.github.io

It forwards to https://michaelgoerz.net.

Moreover, it hosts the documentation for renamed or moved repositories, using a trick pointed out in https://shoehornwithteeth.com/ramblings/2016/12/redirecting-github-pages-after-renaming-a-repository/:

>GitHub allows you to [create public websites in two ways](https://help.github.com/articles/user-organization-and-project-pages/). One [...] is having a specific part of your repo (either a branch or directory) hooked up to the publishing feature. This gives you a URL of `https://your-username.github.io/repo-name/` – where the repo name will always be a subdirectory of the top-level domain.
> The other way is using a repository called `your-username.github.io`. Anything that’s pushed to the master branch in this repo will be visible at (surprise, surprise) `https://your-username.github.io/`, including directories. So you can publish a subdirectory to a top-level repo, or publish to the root of a different repo, and they’ll both be visible as subdirectories of the public domain. [...]
> The `gh-pages` branch (or equivalent) of the project repository will always override the subdirectory of the parent repo (`your-username.github.io`). This is what can use to our advantage, by treating the parent repo as fallback content when renaming the project repo.
