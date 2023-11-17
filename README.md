# Maintaining this site

Download to your local machine and edit with Visual Studio code.

This site makes extensive use of Markdown syntax - recommend installing a  plugin called `Markdown All in One`. It has a mode where you can have a preview window of the generated markdown as you type.

## Running on localhost

The site compiles using a tool called Hugo. Hugo is "a fast and modern static site generator written in Go, and designed to make website creation fun again". Install it using Homebrew.

- https://gohugo.io/
- https://gohugo.io/installation/macos/
- https://gohugo.io/getting-started/quick-start/

To view your site while developing layouts or creating content, cd into your project directory and run:

```sh
hugo server
```

## Running remotely

The site deploys onto Netlify, and if you create a branch and a pull request,
Neflify will automatically create a temporary site where you can see your edits.

Go to e.g. https://app.netlify.com/sites/nifty-ptolemy-7d5b1d/deploys and you will see a panel that says something like:

* Deploy Preview #1: nov-2023-update@60272dc
* Nov 2023 update
* Nov 3 at 6:28 PM

You'll hopefully recognise the name of your pull request!
