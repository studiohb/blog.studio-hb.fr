[![Netlify Status](https://api.netlify.com/api/v1/badges/6f73ae44-1fd4-4a3b-8c84-40652b68aae3/deploy-status)](https://app.netlify.com/sites/blog-studio-hb/deploys)

# blog.studio-hb.com

This blog is powered by [Jekyll](https://jekyllrb.com/) and hosted by [Netlify](https://www.netlify.com/).

You'll find all informations you need on their documentations.

## Getting started

You can add authors in the [config file](https://github.com/studiohb/blog.studio-hb.com/blob/develop/_config.yml) if needed.

To generate a Gravatar hash simply sign up to Gravatar and fill the form here: https://en.gravatar.com/site/check/

### Write a post

To write a post, you need to create a Markdown file in the `_posts` folder. At the very beginning of the file you need to change the [Front Matter](https://jekyllrb.com/docs/front-matter/) config, for instance :

```yml
---
title: My awesome post
layout: post
author: guillaumebriday
categories:
  - My awesome category
  - Another awesome category
image: 2020/07/my-awesome-image.jpg
image_caption: "Photo par: my awesome photographer"
---
```

To display images in the post, you need to include the `image.html` partial, for instance:

```markdown
## My title

{% include image.html img="2020/07/admin-wordpress.png" caption="Interface de WordPress" %}

My content
```

Images are in the [assets/images](https://github.com/studiohb/blog.studio-hb.com/tree/develop/assets/images) folder.

Before uploading, you should resize them (recommended size 1280 * 800 px) and optimize them with [ImageOptim](https://imageoptim.com/mac) (macOS) or [Trimage](https://trimage.org/) (Linux).

## Preview posts locally

Clone the project, then `bundle` to install the required gems

You can then launch the local server and see future posts using:

```
bundle exec jekyll serve --future
```

## Deployment

To deploy the blog on production, you simply need to push on `master`, Netlify handles everything for you.

## Licence

This project is under [MIT](https://opensource.org/licenses/MIT) license.

## About us

<img src="https://www.studio-hb.com/assets/logo-studio-hb-b65681ecbcfbb2c56154ef3da19c09cf20378bb4e341e5f9b57ab319bfec43bc.svg" width="400" />

[Studio HB](https://www.studio-hb.com/) is a Web agency specialized in the custom development.
