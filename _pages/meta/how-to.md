---
layout: page
permalink: how
---

## reminders

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Your first note]]</span> to get started on your exploration.
</p>

- to start serving on `localhost` <br />
open terminal and run command:
```
$ bundle exec jekyll serve
```

- to commit & merge to github:
```
$ git add --all
$ git commit -m 'commit title'
$ git push origin main
```

- make markdown work under HTML class tags: <br />
``<div class="" markdown="1">``

- deploying to netlify from github:

> 1. Log in to Netlify
2. Once logged in, click the “New site from Git” button
3. On the next page, select GitHub as the continuous deployment provider (you may need to authorize the connection, in which case, approve it)
4. On the next page, select your digital garden repository from the list
5. On the next page, keep the default settings, and click on “Deploy site”.