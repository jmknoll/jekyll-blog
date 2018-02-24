---
layout: post-sidebar
date: 2016-08-10
categories: strategy industry
author_name : Jameson
author_url : /author/jameson
author_avatar: fred
show_avatar : true
read_time : 16
feature_image: feature-san-fran
show_related_posts: true
square_related: recommend-san-fran
social-message: Great post over at Writer Theme - You dont have to be great to get started
---

With the continuing explosive growth of javascript and its package manager npm, its getting difficult to decide which new libraries are actually important (signal) and which might seem useful, but will never become industry standards or will shortly fall out of fashion (noise). A couple of thoughts on the state of the industry, and a couple of strategies that I've found useful in filtering out the signal from the noise.

Lets start with the issue. Its an accepted part of a software engineer's job description that you'll need to constantly be learning and practicing new things. However, even if your boss in understanding and lets you mess around with new tech at work, there's a still a pretty hard limit on the amount of time that you can spend learning new tech. Hard as it may to believe, some of us have families, or would rather play videogames than learn the latest javscript framework. So its important to invest your time in tech that isn't going to be dead in the water in six months (look at you, Angular).

Lets look at package managers. I started getting more heavily into SPA development when I joined my current company, Shanghai AppMaker, at the beginning of last year. We did web app development for clients, and our clients (like, I assume, many others) have grown accustomed to Native Apps, and want the web to feel Native. 

Naturally, I needed to learn a framework, and a handful of build tools and generators to go with it. We were using Angular, but Angular on its own isn't sufficient. I also needed bower (for packages), yeoman (for project scaffolding), and grunt (for processing and building). None of these tools are particularly difficult to learn, but they still take time (which is limited). More significantly, none of them turned out to be particularly long-lived, either. Two projects later, my boss had decided that Gulp was better than grunt, and that npm was better than Bower. I agree on both counts, but I still would have rather learned one set of tools. A couple of months later, Browserify was added to Gulp, and then both were swapped out for Webpack. A then React was subbed in for Angular. So we're currently at React and Webpack, and it seems pretty good for now. But both technologies existed when I joined the company, so would have been possible to start with them, rather than waste who-knows-how-many hours of productivity? And just learning the new tech isn't the bad part. Its that constantly switching prevents you from getting into a streamlined routine. 

![view]({{site.url}}/{{site.baseurl}}img/post-assets/view.jpg)

So is there a better way? Or is there a way to evaluate tools with an eye toward the future? I've found a couple of strategies that have proven useful in evaluating tools.

**Who is behind it? And how are they using it?**

The team behind the project is paramount. Take bower and npm as a comparison. Npm had a whole company behind it, whereas bower was just once guy and a couple of contributors. Of course npm was going to be able to pull ahead in terms of features and reliability.

See what kind of activity the project has on github.

For larger projects, look at how the people behind the project are using it. Take Angular and React, for example. Both excellent projects, and both with excellent teams behind them. However, Facebook was actually using React for significant projects (the Instagram website and portions of the Facebook website). They were invested. Google, in comparison, wasn't using Angular for many significant, customer-facing, projects. So it really shouldn't be surprising that React got more investment than Angular. 

**See what devs are talking about**

Around the time I started at the company that I described above, I went to a local JS Meetup. 2 our of the 3 talks that night were about Webpack. The writing was on the wall; I just didn't read it. If enough devs care about something, and think it represents a better way forward, it doesn't seem unreasonable to think that it will see mass adoption. After all, these are the same developers making the choice to adopt a piece of technology, and in most cases, building out the new features and bug fixes. 
 




