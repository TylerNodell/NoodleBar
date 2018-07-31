---
layout: post
title: "Getting Started with Blogging"
date: 2018-07-20 08:55:30 -0400
categories: web development
--- 
# Learning to build a blog with Jekyll

Recently, I've begun my journey to coding competence by starting a coding bootcamp with the Flatiron School in Immersive Web-Development. As part of our course, the instructors want us to build a blog showcasing what we have learned or whatever coding nonsense enters our mind and just wont leave.

But I've never blogged before, hell I don't think I've even followed a blog before. Ironically, the only times I have ever lookled at blogs was to find answers to coding problems I might have had on my own.

## What am I doing?

To be honest I've no idea. I just wanted to make sure that whatever I made I wantd to own and not be hosted somewhere else. I wanted to make sure if somone wanted to see my blog they didn't got to tumblr.com or medium.com, I wanted them to go to TylerNodell.com, or sometehing along those lines. But, I had no idea of what I was getting myself into.

## Jekyll blogging

I had no idea what Jekyll was going into this endevor. All I was looking to do was to figure out a way to avoid tumblr or medium. When looking at a list of options I had for myself, Jekyll seemed like a simple way to implement what I was looking for: a small simple server dedicated to doing one thing, blogging.

## What even is Jekyll?

Jekyll is a static site generator primarily purposed for blogging, meanining it makes a website for you that has the layout of a basic blog. By default it looks much like any blog you can find on medium or tumblr, the magic of Jekyll is that it gives you the freedom of access to the CSS and Javascript files of your blog allowing the user to truely have control of how it looks.

Jekyll creates its posts using the markdown file format, giving the users a wide varieties of tools in order to format their posts. Then the posts are shelled using Liquid, a open-source template programmed in Ruby. 

## How to use Jekyll

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

At this point you can load up your site locally 