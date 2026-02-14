# 💎 crystalblue

a tiny, text-first blog.


## 🧊 what this is

this repo powers the crystalblue blog.

it is a simple static site generated with Hugo and deployed via Cloudflare Pages.

posts live in `content/posts/`.
layouts and styling live in `layouts/` and `assets/`.



## 💭 licences

### blog writing

all blog posts in `content/` are © 2026 crystalblue. all rights reserved.



### site code

all layout, styling, and structural code in this repository (everything outside `content/`) is released under [the Unlicense](https://unlicense.org/). do whatever you like with it.


## 🧿 how to use

if you would like to use crystalblue's sitecode to power your own blog, here is a simple guide.

#### requirements

- git  
- hugo 
- a github account  
- a cloudflare account

#### dev env
1. clone the repo
2. install hugo
3. run it locally with `hugo server -D` (-D shows your draft posts)
4. to write a blog post, run `hugo new content posts/my-post-title.md`
5. edit the file in `content/posts/`
6. commit & push

#### deployment
1. push this repo to github (or fork it).
2. in cloudflare → pages → create project → connect to github.
3. set
* build configuration: `framework preset: hugo`
* build command: `hugo --gc --minify`
* build output directory: `public`
* set environment variable: `HUGO_VERSION = your local hugo version`
4. every push to main now triggers a new deploy


