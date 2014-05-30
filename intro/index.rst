Introduction
============


Welcome to Django Church!
-------------------------

If you're reading this, then it's likely that you're either thinking about using Django Church for your small Church website project, or you've already made the leap! In either case, you're most welcome! This documentation represents the general user manual for managing and maintaining your site's content once it's been set up. If you're after technical documentation about setting up your own Django Church instance, you'll need to go take a look at our `developer docs <http://djangochurch-developer.readthedocs.org>`_. On the other hand, if you want a whistle-stop tour of Django Church's features and interface, you've come to the right place!

This guide starts by exploring Django Church's User Interface (UI). It then takes a look at some basic processes like logging in and changing your password, and lastly covers detailed walk-throughs of each app in turn.

Before you get stuck in we just wanted to say that this guide is not complete! It's a perpetual work in progress. As people ask questions and discover features we haven't fully outlined, we'll add our responses. If you have a query, or have spotted a gap in the guide, please do let us know. The best way to get in touch is by emailing support@blanc.ltd.uk

Onward!


A bit of background
-------------------

What's in a name?
`````````````````

Django Church is so called because it's a Content Management Systems (CMS) for small Church websites, built through a web-application framework called Django, which is an open source tool programmed through the open source programming language called Python.

Why do we need Django Church? Aren't there lots of other content CMS options out there?
```````````````````````````````````````````````````````````````````````````````````````

Good question… we'll overlook that I've just asked it myself. There are many, many, many CMSs out there designed to deliver Churchy-type websites. And there's an order of magnitude more designed to deliver websites generally.

Django Church is non-denominational, and has been developed in association with and funded by the Church of England: Birmingham to enable the future development of small Church websites in a more cost-effective and collaberative way. But, because of its open source nature, anyone from any Church, anywhere in the world can download and use the Django Church code, free of charge.

What sets Django Church apart? There's a few USPs…

It's open source
````````````````

We could go into a lot of detail about what makes something "open source" - we could type for hours in fact. We've written a `paper <http://www.blanc.ltd.uk/downloads/open-source>'_ about open source systems which covers off the core details, but in short, you can think about it like sharing a cooking recipes. Someone develops a recipe and shares it with a few friends. Those friends take the recipe, tweak it, they might improve it but when they are done they share it back amongst their friends, who in turn take, amend and re-share it. In an ideal world, open source philosophy represents a cycle of continuous free and open shared improvement.

Now, amongst the other CMS options there are others built on open source foundations, but few of them - if any - are open source in the purest sense of the word. The majority work on a Software as a Service (SaaS) basis; you rent the site from the provider. They've used open source code and built a proprietary, locked-in CMS. As soon as you top paying rent, your site goes away. We don't think that's the way the Kingdom should work.

Django Church is fully open source. You can visit our Github repository and download it, tweak it, re-share it… with the right skills, you can make it exactly what you need it to be. And if you don't have the skills we can deploy and host it for you. At any point in the futre, you can walk away with your site, and spin up your own copy with the hosting provider of your choice. It's that simple.

What's Python?
``````````````

Python is the programing laguage used to build Django

Python is a serious programmer’s language. It typically doesn’t attract ‘script kiddies’ or designers who’ve picked up other languages like PHP, and learnt what they need to get by. It means that the average Python programmer is significantly more advanced in their understanding and experience of development, re-enforcing point 3 above.

Python enforces consistent programming style, meaning it requires you to write code in a human-readable form, which again reinforces the transferability of code between developers in point 3 above.

Python was a software language long before it was used for web development. It’s a big language designed to solve big problems (see NASA, Google etc.), as a result its support is wide and reaches into industries the world over.

Python scales well. It’s the case that with lesser programming languages like PHP, the bigger the project, the more cumbersome and unstable the platform becomes. Python on the other hand doesn’t suffer from those kinds of bottle-necks.


What's Django?
``````````````

Django is a ‘rapid prototyping’ framework, aided by a huge library of tools and modules pre-built and ready to go. If you want users of your site to be able to log in to the site, you don’t need to build the user-model that manages that process. The models to manage that feature can be added to the project with a line of code. As a result, it’s fast to develop within, enabling rapid turn-around on projects.

Django is incredibly stable and isn’t prone to falling over under pressure.

Django doesn’t make assumptions about your project. Look at Wordpress for a moment. It’s designed to do a fixed set of tasks. It doesn’t matter if you don’t want to make use of those features, they’re still there, clogging up your work flow. Equally, if you want it to do a task that doesn’t feature in its list, you’re stuck. Django lets us build exactly what a client needs and then expand on that long-term. It’s flexible, lean and agile as a result.

It’s being used now, it’s not a bleeding edge piece of technology that’s only supported by three guys in a garage somewhere in Kent. It’s used by mass-market websites like The Guardian, The Onion, Instagram, The Washington Post, NASA and PBS to name just a few.

Django is fast and scalable. There are examples of Django site’s that draw millions of hits a day without blinking.
