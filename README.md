# faux.cab

This is the repo that contains my website for https://faux.cab/. It's basically just a short URL to lead folks to my https://fauxcabulary.org/ website. I only intend the domain to be used for email (e.g. kyle@faux.cab rather than kyle@fauxcabulary.org), but if someone is curious and decides to visit the website, they'll be greeted by something other than a 404 from Github Pages.

## Commands

Here are some recipes for developing, checking code quality, and building a deployable site.

### serve

Run the site in development mode. Edit the sources and see those edits reflected in the local site in seconds. Your site, by default, will be at [http://localhost:8080](http://localhost:8080).

```shell
npm run serve
```

### lint

Run the linter to make sure your code follows some basic formatting and logic constructs.

```shell
npm run lint
```

### build

Build the static HTML that can be deployed to the web server. (Github Pages, for example.) This action generates a production build of the site.

```shell
npm run build
```

### deploy (to Github Pages)

If you've configured your site to serve the `/docs` folder, just commit and push to see your changes live.

```shell
# build the production site
git run build
# see a list of modified, new, and deleted files
git status
# stage your changes in prep for commit/push
git add .
# commit your changes to the local copy of git
git commit -m"more changes for the site"
# ensure there were no upstream changes
git rebase --pull
# push your latest site and source to Github; This will immediately start serving your new edits on Github Pages
git push
```
