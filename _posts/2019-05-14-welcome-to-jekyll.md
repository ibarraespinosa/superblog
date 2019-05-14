---
layout: post
title:  "Welcome to my blog"
date:   2019-05-14 16:31:35 +0800
categories: jekyll update
---

During many years i've had my personal blog hosted on blogger here https://sergioibarra.blogspot.com.br. However, now I'm working on China and www.blogger.com is blocked. Therefore, I created a blog in GitHub because it is not blocked! :laughing:.
Also, in this blog I will post mainly in English, however, in my original blog i use to post on portuguese and spanish.

## Notes about the blog

I will post technical information about R, emissions, air pollution, Julia and bash. I've been using Ubun tu since 2008 as my unique OS, so **do not expect any post for other OS**. Also, I use a lot Git, so please, install it:


{% highlight bash %}
sudo apt install git
{% endhighlight %}



## How to install jekyll

You can find many post around the web how to install jekyll using Baidu, Google, Yahoo, Bing, etc. Here I'm showing a brief summary.

### Get jekyll

{% highlight bash %}
sudo apt install jekyll
{% endhighlight %}

Now you can create a new default blog, like this (better use one word):

{% highlight ruby %}
jekyll new MyNewAwesomeBlog
{% endhighlight %}

**OR**

download a template, as I did on this blog. There are many tempaltes, but I liked this one called space-jekyll-template developed by  ![victor void](https://github.com/victorvoid)

{% highlight bash %}
git clone https://github.com/victorvoid/space-jekyll-template/
mv space-jekyll-template-master MyNewAwesomeBlog
{% endhighlight %}

and that is pretty much it

### Editing

I like a lot Visual Code, so, downlaod it if you want.
Inside the directory of your blog, there is the directory *_posts*. Inside there is a markdown example, where you write the posts:

**2019-05-14-welcome-to-jekyll.md**

The name of the file is strict: YEAR-MONTH-DAY-{BLAHB-LABH}.md
(actually, the extension was .markdown, but I changed it to .md)

So, if you want a new content, just copythe file and save it with another name, respecting the format.

## Super important: *_config.yml*

You must edit the file *_config.yml* according your information. Perhaps, the most important line is **baseurl**. Change it to the name of your blog. Mine is:

**baseurl: "/superblog"**

## Local build to see the blog

{% highlight bash %}
bundle exec jekyll serve
{% endhighlight %}

then enter to http://localhost:4000 to see your page. However, it is cooler to see it on real life.
For more info about jekyll, check here https://jekyllrb.com/docs/ 

## Github Pages.

Create a repository with the same name of the directory of your blog.

Now you can go to your directory and do

(change the word _superblog_ for your blog)

{% highlight bash %}
git init
git add .
git commit -m "first message"
git remote add origin https://github.com/ibarraespinosa/superblog/.git
git push - origin master
{% endhighlight %}

check here

Then go to your repository on Github, click on settings, scroll down and activate your GitHub Pages
with source on your master branch:



## Original content below

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
