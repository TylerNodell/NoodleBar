---
layout: post
title: "Getting Started with Blogging"
date: 2018-07-25 08:55:30 -0400
categories: web development
--- 


# Learning to build a blog with Jekyll
![Pusheen is a blogger](https://thumbs.gfycat.com/AptFirstHartebeest-size_restricted.gif)

Recently, I've begun my journey to coding competence by starting a coding bootcamp with the Flatiron School in Immersive Web-Development. As part of our course, the instructors want us to build a blog showcasing what we have learned or whatever coding nonsense enters our mind and just wont leave.

But I've never blogged before, hell I don't think I've even followed a blog before. Ironically, the only times I have ever lookled at blogs was to find answers to coding problems I might have had on my own.

# What am I doing?

![confused spongyboi](https://thumbs.gfycat.com/GoldenChiefAmericanbittern-size_restricted.gif)

To be honest I've no idea. I just wanted to make sure that whatever I made I wantd to own and not be hosted somewhere else. I wanted to make sure if somone wanted to see my blog they didn't got to tumblr.com or medium.com, I wanted them to go to TylerNodell.com, or sometehing along those lines. But, I had no idea of what I was getting myself into.

# Jekyll blogging

I had no idea what Jekyll was going into this endevor. All I was looking to do was to figure out a way to avoid tumblr or medium. When looking at a list of options I had for myself, Jekyll seemed like a simple way to implement what I was looking for: a small simple server dedicated to doing one thing, blogging.

## What even is Jekyll?

![Jekyll and hyde](https://thumbs.gfycat.com/UnfinishedThankfulDikdik-size_restricted.gif)

Jekyll is a static site generator primarily purposed for blogging, meanining it makes a website for you that has the layout of a basic blog. By default it looks much like any blog you can find on medium or tumblr, the magic of Jekyll is that it gives you the freedom of access to the CSS and Javascript files of your blog allowing the user to truely have control of how it looks.

Jekyll creates its posts using the markdown file format, giving the users a wide varieties of tools in order to format their posts. Then the posts are shelled using Liquid, a open-source template programmed in Ruby. 

## How to use Jekyll

![stackoverflow](https://upload.wikimedia.org/wikipedia/en/f/fa/Stack_Overflow_homepage%2C_Feb_2017.png)

## or

![reddit](https://thumbs.gfycat.com/SoreDecimalKatydid-size_restricted.gif)

Jekyll is simple to start working with but, becomes more difficult depending upon the feature set you desire. For my project I just wanted to start out with a simple base site and work on expanding it in the future. To start with create a repository and cd into it as such.

```
git init <Repository name> && cd <Repository name>
```
Next we need to set up a Gemfile as the are ruby gems, we can do so by creating a new file and giving it our dependencies.

```
source "https://rubygems.org"

gem "jekyll", "~> 3.7.3"

gem "minima", "~> 2.0"

gem "github-pages", group: :jekyll_plugins

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.6"
end
```

After that hop back into terminal and use `bundle install` to load them all in.

Now its time to push everything up to github for basic hosting. Simply add everything into the repository you created then commit and push it.

```
git add * -f

git commit -m "Initial commit"

git push origin master
```

At this point you can load up your site locally on `localhost:4000` to get a feel for what you will see online.

![congrats](https://thumbs.gfycat.com/GraciousShyKid-size_restricted.gif)

Congrats your site is basically up and running, you can start making posts in your posts folder, just be sure to use proper naming conventions.

## How to configure Jekyll

![Code](https://thumbs.gfycat.com/BiodegradableFloweryGreatdane-size_restricted.gif)

By accessing the `config.yml` file the user gains access to the general settings offered my Jekyll.

From here they gain access to:
  1. Blog title
  2. Contact information
  3. Description
  4. Base url a.k.a. the subpath of your site
  5. Hostname and protocols
  6. Social media handles
  7. Markdown style
  8. Jekyll themes
  9. Additional plugins

In addition, everything can be manually edited via the `index.html` files or the `main.css` file in the site directory.

That pretty much sums up Jekyll set up from this point on it is completely up to the user to see what they can do to make a simple website into a blog of their dreams.

Below I've linked, from Jekyll's main site, pages with additional information on themes and plugins.

https://jekyllrb.com/docs/themes/

https://jekyllrb.com/docs/plugins/


![good luck](https://thumbs.gfycat.com/BitterMetallicCommongonolek-size_restricted.gif)