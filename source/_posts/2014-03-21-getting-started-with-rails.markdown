---
layout: post
title: "Getting Started with Rails"
date: 2014-03-21 22:37:58 +0530
comments: true
categories: [Ruby on Rails,Web development,Beginning web development,MVC]
---

You must have probably heard about Ruby on Rails by now. You must have heard people talking about how they wrote an application in less than half the time it would have taken using some other technology. Rails surely is one of the most talked about technology on the internet. But how does it help you developing apps faster? **What is it that makes Rails so popular?** 

In this article I talk about the basic idea behind rails, and how it can help you in your web development.

<!-- more -->

This article basically is the first of the two articles I'm gonna write about getting started with rails. In the current, first article I’ll help prepare you for your first foray into Rails by explaining what it is, how it works, and where it fits into the spectrum of web development and design. Then we get started with some basic concepts and essential components of Ruby on Rails. In the second part (most probably next week) I will try to show how to install the engine. Deploy your first rails app. We will also take a closer look at Rails’ inner workings. Then I’ll point you to some good tutorials on the Web that you can use to learn Rails. I’ll also provide a lot of further reading recommendations so you can dig as deep into the topic as you like.

I assume you’re already familiar with some other form of Web development, whether PHP, Python, Perl or Java, and relational databases like MySQL. First, I’ll introduce Rails and the basic ideas behind it. So lets dive right in.


##What is Rails? {% img right http://upload.wikimedia.org/wikipedia/commons/1/16/Ruby_on_Rails-logo.png  Rails logo %}

Ruby on Rails is a web development framework which was created by [David Heinemeier Hansson](http://david.heinemeierhansson.com/) during [Basecamp’s](https://basecamp.com/) development at 37signals in 2004. Basecamp was built in Ruby because Hansson found PHP and Java not powerful or flexible enough. Hansson wanted make web development easier so he made his own Web development framework, based on simple ideas that had proven successful elsewhere. Rails core foundation is based on pragmatism and established paradigms instead of exotic new ideas. And that’s what made it so successful.

The framework he created proved to be extensible, expandable, and multi-purpose. He decided to share it as open source software. A small group of developers, now known as the Rails Core Team, formed and improved and expanded the framework. After a good deal of effort, Ruby on Rails matured into a robust, solid software development platform. Today, Rails has a strong community and great documentation, and is used by thousands of developers to power hundreds of websites, such as [Twitter](https://twitter.com/), [Github](http://github.com), [Scribd](http://www.scribd.com/), [Hulu](http://www.hulu.com/) and many more.

Rails is designed to make building web applications simpler and easier. Rails provides developers with a large, easily expandable set of building blocks they can use (and re-use) to create web applications. Developers can use, integrate, and customize these components of code in any manner they choose to, to create the unique functionality they need for their application. Building software this way really helps reduce the time it takes for developers to create and later maintain their applications. It also helps to standardize the way applications get built, making it easier for many developers to collaborate and write more uniform code.

###Model-View-Controller

Rails is based on the Model-View-Controller pattern that splits your application into three parts:

 * The **Model** represents the data, and does nothing else. The model does NOT depend on the controller or the view. 
 * The **Views** are the templates that render data to the user and all the logic surrounding presentational aspects of your app. They send user actions (e.g. button clicks) to the controller.
 * The **Controller** sits at the heart of everything, processing requests from clients, initiating changes in the models and triggering the rendering of the templates.

 {% img center http://paceinfonet.org/wp-content/uploads/31.png  Rails logo %}

###Convention over Configuration

David Heinemeier Hansson has referred to rails as _'opinionated software.'_ Rails has strong opinions about how a web application should be composed and how subsystems should be configured together. Unlike existing Java frameworks which rely on reams of XML configuration files, Rails instead believes in __Convention over Configuration__. Ruby on Rails replaces the massive XML configuration files by a consistent naming convention and a standard directory location for the different types of files used in a Rails application.


{% img center http://geekandpoke.typepad.com/geekandpoke/images/2008/06/03/sexpl18.jpg  convention over configuration %}

This means that entities in Rails have to named in a certain conventional way. That’s not to say there’s no possibility of doing things differently if you need to, but you’ll definitely have it easier if you do things **_“the Rails way.”_** And that way happened to be exactly the right one not only for Hansson but for a lot of other developers, too, another important reason for Rails’ success.

### Don't Repeat Yourself (DRY)

Another key philosophical principle behind Ruby on Rails is commonly expressed as **Don't Repeat Yourself (DRY)**. The idea behind _DRYness_ is to minimized duplicate code. At the application level you can reuse Rails code via helpers, or at the language level via class inheritance. Rails also allows for HTML snippet reuse via partials. But in addition to helpers, class inheritance, and partials, Rails has a great plugin mechanism where a you can import and reuse a large set of core Web 2.0 functionality.

{% img center https://i.chzbgr.com/maxW500/1036028672/hF2EBA6B4/  Don't Repeat Yourself %}

##But why Rails?
Now that you have some feel as to what Rails is, lets try to answer the question as why someone should use Rails.

* **Gain from the best practices** : The Rails community set many standards in web development. They pushed new technologies like REST, Unobtrusive Javascript, and so on. They are already using the best practices that are tried and tested. So, for someone new it is better to use these practices than to go your own way.
* **Development speed** : True to its maxime _don’t repeat yourself_, quick development is especially facilitated by getting rid of repetitive coding. Consequently, development cycles in Rails are shorter than those in other programming languages. 
* **Gems/Plugins** :  the Rails community provides a wealth of plugins as Ruby Gems that you simply add to your project Gemfile and install.
* **Testing tools** : Unlike many other web frameworks, Rails supports Testing out of the box.

##Prerequisites for Rails

In general there are really no prerequisites for learning Rails, but I recommend these steps to make your learning curve easier.

1. **Start with Ruby** : It's intuitive to start with Ruby and get familiar with it. When I first started to learn Ruby on Rails. I read a few articles by different bloggers that said that you don’t need Ruby to learn Rails. Well now I see that as totally absurd. Take it from someone who initially took that path. If you take the time to fully understand Ruby before you learn Rails; then learning Rails will become a piece of cake. Whether you build controller, action or else, it will all come down to Ruby. Also get familiar with OOP concepts as ruby is an Object Oriented language(infact everything in ruby is an object) these will help you in understanding ruby better.

2. **Basics of Web develpment** : You will learn Rails much faster if you have some previous web develpment experience, if you are someone new, try to learn atleast basics of internet and web development in general like databases, post , get etc. Another thing I noticed is with Rails you should have some front-end knowledge(basic javascript libraries like jquery, less and sass). You can't be a good Rails developer without some front-end knowledge.

3. **Make command line your friend** : As Most of the time you will be dealing with command line interface while developing apps in rails, try to get familiar with basic commands.

4. **Start using version control** : This is more of a bonus then a prereq. Get familiar with a version control system(preferably [git](http://git-scm.com/)) as most of Rails community uses Git. This will also help you in handling your source code much better. 

I hope this basic introduction to the  Rails gives you some idea as to what Rails is and how it can be useful to your needs. While Rails is already a great platform its still evolving and I see it acquiring a much larger place in the web development space in the future. 

While I have tried to explain all the components as simply as possible, don't worry if you still find it a bit complex. You will get a better feel about Rails once we go into the second part of this article, as it would contain code snippets that you can try on your own, I wanted to first introduce the basic philosophy behind Rails, that's why this article is more of theoretical nature. Once we go into the second part I will take a more of hands-on approach.

In the second part of this tutorial we will get rolling with Ruby on Rails, install the engine, deploy our first rails app and take a closer look at Rails’ inner workings. I will also provide links to some good tutorials and further reading materials on the web. So stay tuned.