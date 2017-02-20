# OCTGN Blog

We use [Hexo](https://hexo.io/) for our blog.

View [Hexo Docs](https://hexo.io/docs) for details on editing

Once you make your edits and you're satisfied, then just [Generate](https://hexo.io/docs/generating.html) the sites files and merge them into gh-pages branch.

## Initial Setup (Windows /w Chocolatey)

#### Install Node.js
You'll probably want to exit your command prompt or powershell after this otherwise the `npm` command won't work

    cinst nodejs

#### Install Hexo
    npm install -g hexo-cli

#### Clone this Repo
    git clone --recursive git@github.com:octgn/blog.git

#### Initialize Hexo
	cd Blog
    npm install