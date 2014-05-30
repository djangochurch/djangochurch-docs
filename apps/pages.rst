Pages
=====

In the majority of cases, pages within a site will account for the vast majority of your content. The Pages app gives you the tool, not only to manage the content on a given page, but to manage the structure of those pages and how they appear to the user.

Managing page and page structures
---------------------------------

1. Click Home > Pages > Pages
2. Toggle between "Tree" and the traditional "Grid" view of pages by clicking the "- view" button in the top-right of the screen.
2. The Pages app has only one model, its self called 'Pages'. It differs from many of the other apps, in that the default "Tree view" of the app's contents is functional. The default Django Church build comes with a rough outline of some of the pages any given Church might find valuable. This also has the benefit of giving you a loose structure to play with while you're getting used to the way Pages work.
3. Each row in the "Tree view" represents a page on your site. Each row (for example **/sunday/ -- This Sunday (edit)** ) will contain the following elements…
    1. **/sunday/** which relates to the pages slug within the site's URL
    2. **Sunday** which relates to the pages title as it will appear in navigation
    3. **(edit)** click to edit the page's content
    4. If a page has related sub pages, these appears as 'nested' trees within their parent. Sub-pages are indicated by the presence of an arrow to the left of the page. Clicking this arrow shows/hides the sub-pages which, when visible, are indented to indicate their parentage.

Ordering pages in "Tree view"
-----------------------------

The "Tree view" its self lets you organise the pages within your site through a simple drag-and-drop mechanism.

1. Click Home > Pages > Pages
2. Find the page you want to organise
3. Click and hold the page's URL or Title elements
4. Dragging the page up and down the list will result in horizontal, blue lines appearing indicating where in the list the page will end up should you let go at a given location.
5. Release the page to drop it into the desired location.

Adding a page
-------------

1. Click Home > Pages > Pages > Add page
2. **URL** defines the portion of the page's URL that appears after your site's domain name, **/about/** for example where the full URL is http://www.church.com/about/. Note that the URL requires leading and trailing slashes: /
3. **Title** defines the publicly visible title which users will see on the site. Try to keep this short and to the point.
4. Navigation gives you mechanisms to manually control where the page appears in the site.
    1. **Parent** enables you to define the page's location directly, rather than using the drag-and-drop tool found in the "Tree view" noted above. Clicking the combo box with give you a list of ALL the pages in the CMS. Moving a page is as simple as clicking the page you want to be the current page's parent.
    2. **Show in navigation** checkbox enables you to hide pages by unchecking. Note that the page is *still live*, but won't appear in public navigation. This means that users of your site can still see the page if they have it bookmarked or, for example, if you email them a link to it.
5. **Content** defines the body content for the page. See `WYSIWYG text editing <http://djangochurch.readthedocs.org/en/latest/start/index.html#wysiwyg-text-editing>`_ for more detail on text options here.
6. Advanced option
    1. **Template name** defines the design template used to display the pages content on the public site. Unless you've had additional page templates designed and built by a `development partner <http://www.blanc.ltd.uk/djangochurch/>`_, "Default" will be the only option available to you.
    2. **Published** check-box defines whether the page is publicly visible on the website. Uncheck this instead of deleting it if the page is no longer needed.
