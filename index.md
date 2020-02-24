---
layout: page
title: Welcome
---

I created this simple site using GitHub Pages and Jekyll.

Will post projects and past work that I have worked on below:

- [Automation with Pytest and Selenium](https://github.com/kevinwlip/Automation.git)

- [GitHub Pages with Jekyll](https://github.com/kevinwlip/GitHub_Pages_Jekyll_Site.git)


<br />
---


Followed this as a guide [simple_site](https://kbroman.org/simple_site)

[Github Pages](https://pages.github.com) provide a simple way to make a
website using
[Markdown](https://daringfireball.net/projects/markdown/) and
[git](https://git-scm.com).

The sites use [Jekyll](https://jekyllrb.com/), a
[ruby](https://www.ruby-lang.org/en/) [gem](https://rubygems.org/), to
convert Markdown files to html, and this part is done
automatically when you push the materials to the `gh-pages` branch
of a GitHub repository.


---
---
layout: page
title: Overview
description: Overview of construction of a website with GitHub Pages
---

The present site is simple, with a style derived from
[JekyllBootstrap](https://jekyllbootstrap.com/) and
[Twitter Bootstrap](https://getbootstrap.com) with a particular
theme. I'll explain how to create a site with exactly this style. If
you want something else, try the
[GitHub Pages](https://pages.github.com) automatic site generator, or
look at the [resources page](pages/resources.html).

These GitHub Pages sites are constructed by having a `gh-pages` branch
of a GitHub repository, with specific files layed out in a specific
way. To see the structure of such a repository, look at the
[repository for the present site](https://github.com/kbroman/simple_site).

    _includes/
    _layouts/
    _plugins/
    assets/
    pages/
    .gitignore
    License.md
    Rakefile
    ReadMe.md
    _config.yml
    index.md

The directories beginning with an underscore contain materials
defining the basic layout and style for the site. If you
[build the site locally](pages/local_test.html) (for testing
purposes), there will also be a `_site/` directory containing the
actual site (with
[Markdown](https://daringfireball.net/projects/markdown/) files
converted to html). You don't want the `_site/` directory in your
repository, so include that in the `.gitignore` file.

The
[`assets/`](https://github.com/kbroman/simple_site/tree/gh-pages/assets)
directory contains any non-Markdown materials for the site (e.g.,
images or example code). These files won't be touched in the
conversion but will be just copied over as-is.

The
[`pages/`](https://github.com/kbroman/simple_site/tree/gh-pages/pages)
directory contains
[Markdown](https://daringfireball.net/projects/markdown/) files that
will become html pages on your site.

The
[`_config.yml`](https://github.com/kbroman/simple_site/blob/gh-pages/_config.yml)
file contains all sorts of configuration parameters (some of which
you'll need to modify). The [`Rakefile`](https://github.com/kbroman/simple_site/blob/gh-pages/Rakefile) contains instructions for
the conversion; you won't modify this file.

It's best to always include
[`License.md`](https://github.com/kbroman/simple_site/tree/gh-pages/License.md)
and
[`ReadMe.md`](https://github.com/kbroman/simple_site/tree/gh-pages/ReadMe.md)
files. But you wouldn't need these to be placed on the website; they'd
just be viewed in the repository on [GitHub](https://github.com). The
[`_config.yml`](https://github.com/kbroman/simple_site/tree/gh-pages/_config.yml)
file contains
[a line sort of like the following](https://github.com/kbroman/simple_site/blob/gh-pages/_config.yml#L5)
(but listing a few more files), indicating files to _not_ move to the
final site.

    exclude: ["ReadMe.md", "Rakefile", "License.md"]

Finally,
[`index.md`](https://raw.githubusercontent.com/kbroman/simple_site/gh-pages/index.md)
is the Markdown version of the main page for your site.

The
[`index.md`](https://raw.githubusercontent.com/kbroman/simple_site/gh-pages/index.md)
file and the Markdown files in
[`pages/`](https://github.com/kbroman/simple_site/blob/gh-pages/pages)
(e.g.,
[the present page](https://raw.githubusercontent.com/kbroman/simple_site/gh-pages/pages/overview.md))
have a header with a particular form:

    ---
    layout: page
    title: simple site
    tagline: Easy websites with GitHub Pages
    description: Minimal tutorial on making a simple website with GitHub Pages
    ---

In the conversion of the site from Markdown to html, this bit says
that the current file is to be converted with the &ldquo;page&rdquo;
layout, and gives the title and the (optional) &ldquo;tagline.&rdquo;
The "`description:`" part gets converted into
`<meta name="description" content="Minimal tutorial on...">`
which, in principle, may be used in the results of google searches.

The rest is basically plain Markdown, though the present site is
configured to use [kramdown](https://kramdown.gettalong.org/) as the
Markdown converter (via
[this line in the `_config.yml` file](https://github.com/kbroman/simple_site/blob/gh-pages/_config.yml#L23)).
Read about the [kramdown syntax](https://kramdown.gettalong.org/syntax.html)
or just look at the
[quick reference](https://kramdown.gettalong.org/quickref.html).

Now go to the page about [how to make an independent website](independent_site.html).

---

# Resources related to GitHub Pages websites


This is a minimal tutorial to get you started. There are lots of
other resources.

- [GitHub Pages](https://pages.github.com)
- [Jekyll](https://jekyllrb.com)
- [JekyllBootstrap](https://jekyllbootstrap.com)
- [Twitter Bootstrap](https://getbootstrap.com)
- [Markdown](https://daringfireball.net/projects/markdown)
- [kramdown](https://kramdown.gettalong.org)

- [Getting a custom domain](https://blog.brooke.science/posts/custom-domain-hosting-with-github-and-namecheap/)
  (by [Brooke Watson](https://blog.brooke.science/))

- [Get started with GitHub Pages (plus bonus Jekyll)](https://24ways.org/2013/get-started-with-github-pages/)
- [Using GitHub Pages to host your website](https://bcreativeweb.blogspot.com/2013/08/using-github-pages-to-host-your-website.html)
- [A guide to using GitHub Pages](https://www.thinkful.com/learn/a-guide-to-using-github-pages/)
- [Using GitHub to power a web project: How and why](https://audreywatters.com/2013/07/07/how-to-run-your-site-on-github/)
- [The power and potential of GitHub Pages](https://konklone.com/post/the-power-and-potential-of-github-pages)
- [GitHub Pages for projects (blog post)](https://blog.aquinzi.com/gh-pages-project/)
- [knitr, github, and a new phase for the lab notebook](http://carlboettiger.info/2012/03/21/knitr-github-and-a-new-phase-for-the-lab-notebook.html)

---

# How to make a personal web page with GitHub Pages

Your [GitHub Pages](https://pages.github.com) sites will appear at

    https://username.github.io/some_site

Of course, this will be with _your_ GitHub user name and with the
names of your GitHub repositories.

I'd recommend putting _something_ at `https://username.github.io`,
since people might look there. (When I started with GitHub Pages, I
thought you were _required_ to have such a site, but either they've
changed things or I'm just mistaken; you don't _need_ this anymore.)

You create one of these sites in much the same way as you
[create an independent GitHub Pages site](independent_site). The only
real differences are

- The repository needs to be called `username.github.io`
- The site sits in the `master` branch rather than the `gh-pages` branch.

_My_ personal site, [kbroman.github.io](https://kbroman.github.io)
(which shows up as [kbroman.org](https://kbroman.org); see the
[GitHub help page on setting up a custom domain](https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages))
is minimal and is actually written in straight html rather than
[Markdown](https://daringfireball.net/projects/markdown/). If you
want, you could just make an edited version of my site:

- Clone my
  [kbroman.github.io repository](https://github.com/kbroman/kbroman.github.io)
- Remove the `.git` directory
- Edit `index.html`, `404.html`, `README.md`, and `License.md`
- Use `git init`, `git add`, `git commit`
- Create a new repository on GitHub named `username.github.io`
- Go back to the command line and do `git remote add` and
  `git push -u origin master`

Alternatively, you could use the procedure I described for
[making an independent website](independent_site.html). The only thing
you do differently is to use the `master` branch rather than a
`gh-pages` branch.

A final note: the `404.html` file will serve as the &ldquo;page not
found&rdquo; page for _all_ of your GitHub Pages (that is, if you
_want_ a personalized 404 page).


