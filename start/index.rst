Getting started
===============


So here's the basics. The next few sections should equip you with all the core information required to learn everything else. We cover everything else *too*, but if your a quick study, the next few sections will see you right.

**NOTE: Everything that follows assumes that you've first started by opening up the web-browser of your choice. Everything after the section called "Logging in" assumes that you have, in fact, logged in.**

Logging in
----------

1. Start by visiting the home page of your website. Let's, for the sake of argument, say that your site's URL is http://www.example.org
2. To get to the administration dashboard (admin for short) all you have to do is add /admin/ to that URL - http://www.example.org/admin/ - and hit return.
3. You'll then see a login screen with "Username" and "Password" fields. Type these details in and click "log in."
4. If all is well, you should now be looking at a page headed "Django Church administration"
5. If this is the first time you've logged in, it might be a good idea to update your password with something super-memorable and equally secure. You can do this by clicking "Change password", located in the top right of the screen. See the "Changing your password" section below for more.


Apps and models
---------------
All the functionality in Django Church breaks down into individual applications (apps) which deal with specific areas of functionality. The apps installed with the core Django Church package which you have access to, are listed in white text in blue bars. These are things like "Assets," "Events" and "Pages".

Beneath each app, you'll see individual models which relate to more granular areas of functionality. typically these contain lists of things, so for example, the "Images" model under the "Assets" app contains a list of all the images that have been uploaded for use on the website.

You can click on the App name which will drill you into a refined view of the models available to you. You can also click directly the model names to jump to their list views.

Django Church allows admin Super-users to restrict access of particular features of the site to other users of the site. The typical example might be that a several users are commissioned to keep the website up to date - and so need access to edit pages etc. - but won't need to add events to the system.

Knowing this is important, in that the apps and model you see when you log in, will depend on the actions your profile has been given access to.


UI basics
---------

Django Church's UI is entirly consistent. If you see a button called the same thing as one you've seen elsewhere, it's a sure bet that'll do what you expect it to do. In our experience, this means that once a user has understood one section of the site, the rest of the system tends to be an open book to them.

It's worth noting that the majority of the UI conventions we'll talk about here are stock Django conventions which we inherit. Here's a few of the UI conventions it's helpful to bare in mind…

Required/Options
````````````````

One of the simplest things to point to, one of the easiest things to overlook. when you're looking at a form, let's use the news post form (Home > News > Posts > Add post) for example. Look at the the field labels running down the left side of the form. Note that "Title," "Category" and "Date" are all **bold** while "Image" and "Teaser" are not. That's because **bold** field labels denote required form elements while non-bold ones are optional.

The green +
```````````

In short, a green + symbol next to an object gives you quick access to dialogues that you add one more of this kind of thing to the system. You can find them on each model row on the admin dashboard, giving you quick access to adding things without having to first click through to the list view.

You may also see them within larger forms where apps and models are cross-referencing each other. A good example of this is to be found with the "Add image" form in the Assets app (Home > Assets > Images > Add image). Alongside the "Category" combo-box, you'll see the green +, clicking it will let you quickly add a new category to the combo-box without having to back out of adding the image and go back into the "Categories" model.

The three saves
```````````````

At the bottom of every form you'll find the same three save options, and they all have their uses…

1. "Save," typically high-lit in blue. Clicking this button saves the form and takes you back to the model list.
2. "Save and continue editing" is incredibly useful. It's like hitting control-S while you're working on a Word doc; it saves the contents of the form, but keeps you on the form so you can continue your work without fear of loosing a large volume of work.
3. "Save and add another" saves the form and then takes you to a fresh, empty form ready for you to add another. This is particularly useful when you are adding multiple instances of a type of thing in a single session.

What? No cancel button?
```````````````````````

Yep; no. Django doesn't bother cluttering up your window with redundant buttons. If you've started something and you realise you don't want to bother saving it, just navigate away from the page by hitting your browser back button, of clicking the pebble-trail near the top-left of the screen. Nothing is saved until you save.


Changing your password
----------------------

It's a really, really good idea to keep your password safe, secret and as cryptic and/or random as you can manage. We can't help you with that bit, but here's how you get there…

1. From any page within the admin, click "Change password" in the top-right of the screen.
2. You'll be presented with a form, first of all type your "Old password," this will confirm that you are who you say you are.
3. Then type your "New password."
4. Then type it a second time to confirm that you definitely got it right.
5. Click "Change my password" and you're done!


Where should I put my content?
------------------------------

This question isn't strictly about the use of the CMS, but about content and where you should keep it. It might seam obvious but it's often the case that, even though the apps are all labeled as to what their function is, user put content into the wrong area of the system. Sometimes event content ends up in a news story because the user rationalises that they want to tell a story about it; or more commonly, bite-sized news content ends up in general page content, over-complicating navigation and cluttering up the place.

The reality is, all three main content apps - pages, news and events - are capable of containing images, descriptive text, location information and date/time information. As a result, it's not always clear where a given bit of content should live.

We do a lot of Information Architecture (IA) work, and this issue goes to the heart of that discipline. It's complex and it's another subject I could write for hours on, but for a novice, the basic thrust can be summed up in one question: **What is the most important thing I need people to understand about this bit of content?**

If the answer to that question is "the most important thing about this bit of content is this future date," it's probably an event, and so the events section is the right place for that content.

If the answer is "it's about telling people about a thing that happened or is going to happen" -but the date is secondary, it's probably news.

And lastly, if the answer is "it's about making sure people find this content because it's about who we are," then that sounds like a page, at least because pages automatically appear in the site's navigation, so it elevates it in terms of perceived importance.

There are no absolute rules in all of this, and users typically find their way around these themes over time. The important thing is consistency.


URL character limitations
-------------------------

A note on best practice for constructing URLs. A number of the sections below deal with URLs for object, both uploaded to the system, and defined by it through "slug" and "URL" fields on particular forms.

If you remember one thing, remember this: **don't use spaces in slugs and URLs. Use dashes - or underscores _ instead.** It's likely that constructing a slug or URL with spaces will break things for at least some users on certain browsers.

So what characters are safe? In short, all alpha-numeric characters, plus a few punctuation marks. In practice you should limit your characters to…

abcdefghijklmnopqrstuvwxyz
ABCDEFGHIJKLMNOPQRSTUVWXYZ
1234567890-_./

…and where possible, don't use upper-case letters at all.

.. _wysiwyg-text-editing:

WYSIWYG text editing
--------------------

What You See Is What You Get, or WYSIWYG (pronounced "wizzy-wig"), is the label we apply to tools which write HTML code for you online. They give you a Word-like experience of editing content, without having to bother with learning to format text through abstract HTML tags. There are many WYSIWYG editors out there, but Django Church uses `Redactor <http://imperavi.com/redactor/>`_. It strikes a great balance between robustness and offering common tools which most users might need.

There are three places where you can find WYSIWYG text editors within Django; events, news and pages. The rules are the same no matter where you are editing content, so rather than duplicate this section of the guide three times, this is your single reference point.

Limitations
```````````

The first thing to say is that WYSIWYG text editing is not an exact science. No one editor has it exactly right, and so as developers you have to choose the editor that best fits your project. However, this does mean that occasionally, you might need to look under the hood of the editor at the HTML it's writing for you. If that prospect scares you, don't worry, that's what support is for!

Best practice in writing your content
`````````````````````````````````````

In an ideal world, users of the system would type their content directly into the context where it was being used. In practice people tend to write their content in Word, and then copy/paste it into the web browser. The problem here is that Word uses tags that look like HTML to define its text formatting. Unfortunately while the tags look like HTML, they aren't and pasting direct from Word to a WYSIWYG editor can scramble your text completely. If you do write your content in Word, it's worth copying and pasting it into a TXT editor like Notepad, then copying it again from Notepad and only then pasting it into your WYSIWYG editor. It sounds a bit contrived, but it will have the effect of stripping out all the HTML-like tags Word uses.

If you have to use an external editor, consider using an app like Notepad by default. The reality is, all your formatting of headlines and bullet-lists etc. will need to be re-done in the CMS anyway, so there's no benefit to styling your text before it gets to that point.

Formatting options.
```````````````````

1. Click Home > News > Posts > Add post
2. Half way down the page you'll see the **Content** section. Along the top of the large text field that follows, you'll say a row of button icons. These are the control dialogues for your content. From left to right…

    1. **</>** is the HTML/Preview toggle. It lets your switch between the default WYSIWYG preview and the HTML beneath it. *Unless you know what you're doing, it's inadvisable to edit the HTML directly.* That said, it can be helpful to take a peak every now and then as it's really not that hard to pick up.
    2. **¶** is called a "pilcrow" and is short-hand for "paragraph". This button gives you access to the various pre-defined headline and paragraph styles. Clicking it presents a drop-down list of the options rendered in an appropriate style - if not the fonts or colours they will finally be rendered in on your site. To apply a style, simply place your curser within the paragraph you want to affect, and select an option from that drop-down. Note that the style will effect the entire paragraph.
    3. **B** makes selected text bold.
    4. **I** makes selected text italic.
    5. Struck-through **T** makes selected text struck-through
    6. The next two icons relate to bulleted and numbered lists respectively. Clicking either will create a list when on the line where the curser is sat, or alternatively, selecting a body of text will convert each paragraph selected into a bullet when clicked.
    7. The next two icons relate to indentation of paragraphs. to indent or outdent a para, simply place the cursor within the paragraph and click the appropriate icon.
    8. The **Insert image** (picture frame) icon lets you embed images inline with your text.

        1. When clicked, it presents an input field which is expecting the full URL of the image.
        2. If you are linking to an image in the Assets app, all you need to do is to open a new browser window (or tab) and navigate to the assets list (Home > Assets > Images), and then copy/paste the URL of the desired image from the "Location" column.
        3. Clicking "Insert" embeds the image at the location of your cursor.
        4. *NOTE that the image should be as close to the dimensions as you intend to use them as possible.* Uploading larger image will result in very slow page-loads.

    9. The **Insert video** (play symbol in a rectangle) icon lets you embed videos from third party streaming services such as YouTube within your content.

        1. When clicked, it presents an input field which is expecting the EMBED code which most providers supply.
        2. Clicking "Insert" embeds the image at the location of your cursor.
        3. For more information around embedding such content, please consult with your provider of choice for the best results.

    10. The **Table grid** icon enables you to create more complex tables of information within your page content.
    11. The **Chain-link** icon enables you to assign hyperlinks to text within you content.

        1. First select the text you want to be clickable.
        2. Then click the icon, it will present input fields which define the URL you want users to see when they click.
        3. If you want the link to open in a new window, check the "Open link in new tab" checkbox
        4. Click "Insert"

    12. **Underlined A** allows you to pick a colour for the selected body text. *NOTE: Colours are assigned by the CMS Style-sheets. You should not need to assign colours manually in most cases.*
    13. **A in a Box** allows you to pick a colour for the background of the selected body text. *NOTE: Colours are assigned by the CMS Style-sheets. You should not need to assign colours manually in most cases.*
    14. The last but one icon lets you set the text **Alignment** for selected text.
    15. The **—** icon allows you to insert scores into text, which can be used to structure information on long pages of content.

Those are the building blocks. There's nothing like experimentation and exploration to help you get to grips with these tools, so we recommend sitting down with some sample content and playing with it.
