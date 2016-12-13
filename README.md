# Hugo Foundation v6 Blog
A simple [Hugo](https://gohugo.io) theme based on the [Foundation v6 blog (w/ sidebar) example](http://foundation.zurb.com/templates-previews-sites-f6/blog.html), with build tools from [Foundation Zurb Template](https://github.com/zurb/foundation-zurb-template/)

![Screenshot](https://raw.githubusercontent.com/htko89/hugo-theme-foundation6-blog/master/screenshot@2x.png "Screenshot")

## Warning: 
> This repository is not ready for production, or release.
> Disregard Below - All files / instructions are yet to be overwritten with relevant Foundation code / info.

## Features 
* Responsive design
* Uses Bootstrap v4's [native system fonts](http://v4-alpha.getbootstrap.com/content/reboot/#native-font-stack) to load quickly and look good on all platforms
* Basic [OpenGraph](http://ogp.me) and [Twitter Card](https://dev.twitter.com/cards/types) metadata support
* robots.txt linking to XML sitemap (disabled by default, see [Hugo docs](https://gohugo.io/extras/robots-txt/))
* Basic support for [multi-lingual content](https://github.com/spf13/hugo/blob/master/docs/content/content/multilingual.md) (added in Hugo 0.17)
* Supports Google, Bing, and Yandex site verification via meta tags
* Supports Google Analytics (async version), see [Hugo docs](https://gohugo.io/extras/analytics/)
* Supports Disqus comments, see [Hugo docs](https://gohugo.io/extras/comments/)
* Can show a message about cookie usage to the user, see [`exampleSite/config.toml`](https://github.com/htko89/hugo-theme-foundation6-blog/blob/master/exampleSite/config.toml)
* Allow addition of custom `<head>` code in site's `layouts/partial/head-custom.html` (see [#17](https://github.com/alanorth/hugo-theme-bootstrap4-blog/pull/17))

## Usage
Clone the repository to your site's `themes` directory. Refer to [`exampleSite/config.toml`](https://github.com/htko89/hugo-theme-foundation6-blog/blob/master/exampleSite/config.toml) for optional configuration values. A few suggestions to help you get a good looking site quickly:
* Keep blog posts in the `content/post` directory, for example: `content/post/my-first-post.md`
* Keep static pages in the `content` directory, for example: `content/about.md`
* Keep media like images in the `static` directory, for example: `static/2016/10/screenshot.png`
* If you want an image to be shown when you share a post on social media, specify at least one image in the post's front matter, for example: `images: ["/2016/10/screenshot.png"]`
* Use the `<!--more-->` tag in posts to control how much of a post is shown on summary pages

## Building, for developers. (Optional)
This theme uses the build tools from [Foundation Zurb Template](https://github.com/zurb/foundation-zurb-template/) framework, for plain and simple scss / js building. For building, we have three directories:
* `/static` contains built css / js files for immediate use.
* `/source` contains unbuilt scss / js files.
* `/bin` contains foundation's node and bower modules. 
* To set up a build environment, run the following from the `/bin` directory.
```
$ npm install
$ bower install
```
* Then, to build debug css / js: (not minifed)
```
$ npm run start
```
* Or, to build production css / js: (minified, sourcemapped)
```
$ npm run build
```

## Contributing
There are several ways to help with the development of the theme:

* [Open an issue](https://github.com/htko89/hugo-theme-foundation6-blog/issues/new) on GitHub if you have problems or feature requests
* Alternatively, tackle one of the [existing issues](https://github.com/htko89/hugo-theme-foundation6-blog/issues) on the issue tracker
* Fork [the repository](https://github.com/htko89/hugo-theme-foundation6-blog) on GitHub, add features on a "feature" branch like `update-bootstrap`, and then send a [pull request](https://github.com/htko89/hugo-theme-foundation6-blog/compare) with your changes

## License

### This repository is maintained by:
* [Tony Ko](https://github.com/htko89), 
  * [GPL 3](https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)) - [License file](https://github.com/htko89/hugo-theme-foundation6-blog/blob/master/LICENSE.txt)

### This repository was originally forked (now cloned) from:
* [Alan Orth - hugo-theme-bootstrap4-blog](https://github.com/alanorth/hugo-theme-bootstrap4-blog/)
  * [GPL 3](https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)) - [License file](https://github.com/alanorth/hugo-theme-bootstrap4-blog/blob/master/LICENSE.txt)
  * Clone rationale: Foundation framework and demo implementation are different enough from original theme by Alan to possibly necessitate licensing, hence a new repository.

### This repository contains the code of:
* [Foundation Zurb Template](https://github.com/zurb/foundation-zurb-template/)
  * [MIT license](https://tldrlegal.com/license/mit-license)
* (In process of removal from repository) [Bootstrap](http://getbootstrap.com/)
  * [MIT license](https://tldrlegal.com/license/mit-license)
* (In process of removal from repository) [Font Awesome](http://fontawesome.io/)
  * [Various licenses](http://fontawesome.io/license/).
