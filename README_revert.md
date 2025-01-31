

## features
 1. Google Analytics
 2. Dark mode
 3. Disqus comments
 4. Categorization
 5. Emojis Support
 6. Highly optimized blog
    

## Desktop Preview

![Home Page](/screenshots/Home.png?raw=true "Home View of the website")

![Blog List Page](/screenshots/Blog.png?raw=true "Blog List of the website")

## Mobile Preview

![Home Page](/screenshots/Home-Mobile.png?raw=true "Home View of the website")

![Blog List Page](/screenshots/Blog-Mobile.png?raw=true "Blog List of the website")


## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "dev-portfolio-blog"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: dev-portfolio-blog
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install dev-portfolio-blog

## Usage

To start using the theme you either follow these steps or simply fork my repo https://github.com/rohitjain00/rohitjain00.github.io and update the files.

### Recommended
 Please use the theme as the plugin so that all the latest updated for this theme comes directly in your website.

#### Clone the branch `master` and change the theme accordingly.


### Starting from the beginning:
Assuming that you started your first website based on `minima` theme from [here](https://jekyllrb.com/docs/)

1. Add a `favicon.ico` to the root directory for favicon.

2. Create `blog.md` in the root folder ans set its yaml parameters to

```yaml
layout: blog
permalink: /blog/
title: [Blog Page Title]
pagination:
  enabled: true
```

3. Change your `about.md` yaml parameters to following

```yaml
layout: description
permalink: /about/
title: About
```

3. In the `index.md` file add

```yaml
layout: home
home_text: Text
title: [Home Page Title]
```

4. Create a new `categories.md` file in root with following yaml parameters
```yaml
layout: categories
permalink: /categories/
title: Categories
```

4. In the `_config.yml` file add following and change accordingly

Path is relative to the root directory
```yaml
resume_url: [PATH_TO_RESUME]
author_name: [YOUR_NAME]
description: [SITE_DESCRIPTION]
url: [WEBSITE_URL]
google_analytics: '[google analytics Id]'
disqus:
    shortname: [discus-shotname]
```

### Minifier

Visit [Jekyll-minifier](https://github.com/digitalsparky/jekyll-minifier) and add this to your `_config.yml` file to enable minifier.

### Pagination

Visit [jekyll-paginate-v2](https://github.com/sverrirs/jekyll-paginate-v2/blob/master/README-GENERATOR.md#site-configuration) and add this to your `_config.yml` file to enable pagination.

### Check here [_config.yml](https://github.com/rohitjain00/rohitjain00.github.io/blob/site/_config.yml) for example config file.


## Writing a new blog

Create a new folder `_posts` in root folder if not already exists.

1. Create a new markdown file in the format `yyyy-mm-dd-postname.md`
2. Make sure that disqus's shortname is valid.
3. Add yaml configuartion to the post

```yaml
---
layout: post
comments: [true | false]
title: Hello World
categories: [category1, category2]
---
Post Text.
```

## Troubleshooting
- ` Could not find a JavaScript runtime. See https://github.com/rails/execjs for a list of available runtimes`
   Node JS is missing from your system. In ubuntu install using `sudo apt-get install nodejs` or refer to [this](https://stackoverflow.com/questions/9202324/execjs-could-not-find-a-javascript-runtime-but-execjs-and-therubyracer-are-in)


## Contributing

Bug reports and pull requests are welcome on GitHub at <https://github.com/rohitjain00/dev-portfolio-blog/.> This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `dev-portfolio-blog.gemspec` accordingly.

### Read about the themes and how it's implemented [here](https://github.com/rohitjain00/dev-portfolio-blog/wiki/Theme-Management)

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).