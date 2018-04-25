---
layout: post
date: 2015-02-11 08:50:28
categories: coding tutorial
author_name : Jameson Knoll
author_url : /author/jameson
author_avatar: jameson
show_avatar : true
read_time : 10
feature_image: feature-laptop
show_related_posts: true
square_related: recommend-laptop
---

Deploying a React component demo page to Github Pages

So you built yourself a nice React component in your latest project, and now you're ready to show it off to the world and hopefully give back to the community with a well-documented, well-maintained npm package? You're in luck, because I just went through this process myself, and after a bit of trial and error, think I've hit on a pretty good process to make everything run smoothly. 

The entire process is basically just three steps. 1) Pull the component out into a standalone application. 2) Make a demo page which incorporates your component. 3) Deploy the demo page to github pages and the package to npm. 

1) Pull the component out into a standalone application.

If you're anything like me, you didn't set out to make a React component for public consumption. Rather, you were working on a project, needed some functionality that wasn't well-covered by an existing library, and rolled your own. So before you can do anything else, you need to copy your component from your existing project and get it running on its own. 

The easiest way to do this is start a new react project and bundle/serve it with webpack. If you're not familiar with Webpack, this guide does an excellent job of walking you through the setup of a simple react project. https://www.valentinog.com/blog/react-webpack-babel/#How_to_set_up_React_Webpack_and_Babel_setting_up_the_project

You're essentially just creating a single js file which loads react and your component, and mounts it to a `root` element in your index.html in order to serve your component. As you're setting this up, its important to keep in mind that we're really making two different things here. What you're setting up in this guide will become the demo page for your project, and will import your component, but will not actually be part of the component that gets deployed to npm. So make sure to keep them entirely separate for now, and linked only by a single import statement. 


---

Jekyll also offers powerful support for code snippets:

{% highlight javascript %}
{
  "name": "my-project-name",
  "version": "0.1.0",
  "devDependencies": {
    "grunt": "~0.4.5",
    "grunt-contrib-jshint": "~0.10.0",
    "grunt-contrib-nodeunit": "~0.4.1",
    "grunt-contrib-uglify": "~0.5.0"
  }
}
{% endhighlight %}

The easiest way to add Grunt and gruntplugins to an existing `package.json` is with the command `npm install <module> --save-dev`. Not only will this install `<module>` locally, but it will automatically be added to the devDependencies section, using a tilde version range.

For example, this will install the latest version of Grunt in your project folder, adding it to your devDependencies:

Grunt
