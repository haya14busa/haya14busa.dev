+++
date = 2021-01-10T11:00:00Z
lastmod = 2021-01-10T11:00:00Z
author = "default"
title = "Built my static tech blog site using Hugo, Netlify, and GitHub"
subtitle = "My first post in this blog and why and how I built it"
feature = ""
tags = ['haya14busa.dev', 'hugo', 'netlify', 'github-discussions']
toc = true
slug = 'my-first-post'
discussion = 'https://github.com/haya14busa/haya14busa.dev/discussions/5'
draft = false
+++

## Built my shiny personal blog! :sparkles:
I used [Medium](https://medium.com/@haya14busa) so far for English blog posts,
but I now built my shiny new blog site! Yay! :sparkles:

I plan to write about my various OSS projects like reviewdog or Vim plugins,
with more personal things occasionally.

## Technology Stacks
I chose [Hugo](https://gohugo.io/) for static-site generator and
[Netlify](https://www.netlify.com/) as a hosting service.
The source of this blog is in GitHub ([haya14busa/haya14busa.dev](https://github.com/haya14busa/haya14busa.dev))
and Netlify will automatically build and deploy posts on push.

### Why? Stability/Maintainability matters!
I also considered using other tools like Gatsby or Nextjs/Nuxtjs as
a static-site generator. The frontend ecosystem is continuously evolving, and I
felt it could be good to use such technologies for learning purposes.

However, I decided to use Hugo because my top priority for the blog
is stability and maintainability. Hugo is written in Go, which I mostly use, so
it should be easier for me to investigate Hugo's code if needed.
I suppose Hugo should be relatively stable compared to the other tools. It
existed from 2013 and is still actively maintained. I wouldn't say other
frameworks are not stable or difficult to maintain (I didn't fully investigate
them), but I bet on Hugo :)

Hugo is the fastest framework to build static-site too :zap:
I didn't test/compare other frameworks on my own, though.

### Side-story: My wrong choice in the past ... Octopress
I actually already have my personal blog in Japanese (http://haya14busa.com)
which I built loooong long ago (2014).
It's built with [octopress](https://github.com/octopress/octopress) as of
writing. Octopress is a kind of wrapper of [Jekyll](https://github.com/jekyll/jekyll).

At that time, Jekyll was a hot framework because it's supported for GitHub Pages
and Octopress looks very cool to me as it complements missing features of Jekyll
for managing a blog.

However... it turned out it was very painful to maintain. I couldn't follow the
breaking changes of Octopress, and it was actually difficult to follow.
I couldn't catch all errors on build, for example.
Ruby was not my language, and I'm not so familiar with Ruby nor gem/bundler too.
I was fed up with resolving bundler set up failures, which I believe
is easier nowadays, but it was not simple at that time.

... and Octopress maintenance completely stopped.

It was painful but became an interesting lesson for me.

## Hugo Theme: Axiom+
The Hugo Theme is Axiom+, which is my fork version of the
[Axiom](https://github.com/marketempower/axiom) theme. I found Axiom theme in
Hugo Themes site, and I loved it, but there are several missing features I'd like
to have in my blog site, so I forked it and added the following features.

### Features
You can compare this blog and [the Axiom Example](https://axiom-example.netlify.app/) if you're curious.

- **Sticky Table Of Contents**
  - Note that it's not sticky from mobile, though.
- **#tags** at the top of a post
- An author's **social links** (Twitter and GitHub) at the top of a post.
- **Suggest Edits on GitHub** (added a link at the last of posts)
- **Discussions on GitHub** (added a link at the last of posts. See the below section.)
- Share buttons position: from top to the bottom of a post.
  - Because I'd like you to read the post before sharing it :)
- Atom Feed Icon
	- I'm not sure whether people still use RSS/Atom feed, though.

I may contribute the above features back to the original Axiom theme later, but
I just forked it, at least for now, as they are not small changes and wanted to
publish my blog first.

## Experimental: GitHub Discussions as discussion/comment/feedback platform
I believe it's very important to have a place to discuss a post. You should
be able to discuss a post with others, including the author. Or you can just
read other's discussion or leave feedback.

Reddit and Hackernews are good platforms for this purpose, but we cannot always
submit a post to them for every blog post, so I'd like to try using [GitHub
Discussions](https://github.com/haya14busa/haya14busa.dev/discussions/)
as a default discussion/comment/feedback platform for this blog.

I assume readers of my blog are mostly software developers and have their
GitHub account.
You can use markdown including code syntax highlight in comments, can leave
feedback as reactions with ease, and the source of this blog is in GitHub as
well.
I believe it's suited :)

## Next...
I don't decide yet but related to this post, next I plan to ...
- built a static (blog) web site for [reviewdog organization](https://github.com/reviewdog)
  and use a similar setup with this blog if it works well.
- set up GitHub Actions in this blog repository for automated proofreading using reviewdog.

I may or may not write a blog post about it but not sure. We'll see :)

Follow me on [Twitter](https://twitter.com/__haya14busa__) to receive a tweet of
a new post and leave any comments/feedback about this post in [GitHub discussion](https://github.com/haya14busa/haya14busa.dev/discussions/5)!
