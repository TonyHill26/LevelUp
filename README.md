# Deploy Status

[![Netlify Status](https://api.netlify.com/api/v1/badges/f1a4de7b-5717-48b6-8a54-e5466faf45a6/deploy-status)](https://app.netlify.com/sites/nifty-ptolemy-7d5b1d/deploys)

# Maintaining this site

Download to your local machine and edit with Visual Studio code.

This site makes extensive use of Markdown syntax - recommend installing a  plugin called `Markdown All in One`. It has a mode where you can have a preview window of the generated markdown as you type.

## Running on localhost

This new version of the site uses Hugo Blox builder. There's a useful page at https://docs.hugoblox.com/getting-started/page-builder/ which explains how it all works.

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

## Draft posts

To write a draft post, add the following to the top section of your post:
```
draft: true
```

Then run `hugo server --buildDrafts` to see the post.

Or - you can create a branch and pull request, to create a pre-release version you can share with others on a hidden Neflify URL.

Remember to remove the `draft: true`!

## DNS Records

Please see [DNS Records](dns-records.md) for the Netlify DNS records.
