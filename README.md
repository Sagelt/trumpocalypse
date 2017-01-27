# trumpocalypse
_Tracking our slide_

trumpocalypse is a way of tracking what isn't normal around us. It's designed to be easy-to-use, distributed, and customizable.

This repo provides YAML-formatted data to track the abnormal things happening under the Trump presidency. On its own it's just a data store, but if you have a [Jekyll](https://jekyllrb.com/) site you can use this data along with [a page template](https://github.com/Sagelt/trumpocalypse-ui) to keep your own log.

trumpocalypse is designed to be easy to merge in to, to enable sharing of posts between people. Each person can keep their own repo and take or ignore pulls as they feel fit. This isn't an editorial service, it's a method for people to keep their own logs and share how they want to.

## Using trumpocalypse on Jekyll with this repo

These steps assume you have an existing Jekyll site. If you don't, [GitHub pages](https://pages.github.com/) is a great way to set one up.

1. Add trumpocalypse as a submodule within your \_data directory
```
git submodule add https://github.com/Sagelt/trumpocalypse.git trumpocalypse
```
2. Add trumpocalypse renderer as a submodule wherever you'd like the page to live. For example, if you add the submodule under /pages, you'd run this command there.
```
git submodule add https://github.com/Sagelt/trumpocalypse-ui.git trumpocalypse
```
3. Update as often as you'd like
```
git submodule update --remote
```

## Using trumpocalypse on Jekyll with your own repo

As above, but replace the repo links being added with your own repos.

## Pull Requests

Please send your pull requests! Note that taking pulls to this repo is my personal decision. If you don't like the things I choose to highlight you can use this system to make your own.

Each story should go in its own .yaml file in a directory based on the date. title and url fields are required, at least one tag is recommended. desc field is optional.

Stories are displayed in alphabetical order based on file name. Place your files in whatever order makes the most sense to you.

## FAQ

### WHY?

Some friends and I have a group chat where we share news stories. [garykac](https://github.com/garykac) had the great idea of hosting a page to collect all these things. It resonated with me because I'd heard advice to keep a log of changes to avoid the slow redefinition of 'normal' under Trump. I wanted to make something that could be merged easily so people can share what they find, so I expanded on garykac's idea.

### Did you just reinvent CMS on git with static HTML and YAML?

Yep. 

### Why Jekyll/Git/YAML/Bootstrap instead of X/Y/Z?

I used stuff I like. I was more interested in creating a tool anyone could fork and host themselves than fancy CMS features.
