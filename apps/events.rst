Events
======

Just FYI, the events section of the CMS is one of its more complex. structuring events generally isn't easy, and so we've sought to break it down into a structure that would make sense to most users - on both the admin *and* on the public sides of your site. 

Events models
-------------

As a result we've split events as a general content type, into two groupes. Firstly, recurring events which happen every week - Sunday services for example - and secondly, special events which only happen once and/or less regularly than once a week.

Recurring events
----------------

1. Click Home > Events > Recurring events
2. Here are listed all the regular events currently available in the system.
3. Each event presents the following bits of meta, from left to right…
    1. Title (click here to view)
    2. Day of the week (Monday, Tuesday. etc.)
    3. Published (indicates whether or not the event is visible to the public)
4. To edit an existing event, click the event title.
5. To add a new event, click "Add recurring event".

Add a recurring event
---------------------

1. Click Home > Events > Recurring events > Add recurring event
2. **Title** defines the title of the event. Note that this is the publicly visible title users of the site will see
3. **Image** is an optional field that lets you define a key image to associate with the event. This is achieved by selecting an image from the Image Assets app through the combo-box.
4. **Description** defines the descriptive text about the event which is seen when users navigate through to the event's detail page.
5. **Day of the week** The combo-box defines the kind of breakfast you'd like on that day… kidding. It defines the day of the week the event happens on.
6. **Frequency** is a fuzzy field designed to give users an indication of how regularly the event happens. "Weekly" or "fortnightly" for example.
7. **Published** check-box defines whether the event is publicly visible on the website. Uncheck this instead of deleting it if the event is no longer needed.

Special events
--------------

1. Click Home > Events > Special events
2. Here are listed all the special events currently available in the system.
3. Each event presents the following bits of meta, from left to right…
    1. Title (click here to view)
    2. Start (the start date and time of the event)
    3. Published (indicates whether or not the event is visible to the public)
4. To edit an existing event, click the event title.
5. To add a new event, click "Add special event".

Adding a special event
----------------------

1. Click Home > Events > Special events > Add special event
2. **Title** defines the title of the event. Note that this is the publicly visible title users of the site will see
3. **Slug** which refers to the human-readable portion of the event’s URL once it’s live.
    1. For example an event with the slug “coffee-morning”, the resulting URL would be this “http://www.example.org/events/view/special-event/”.
    2. Note that standard URL character limitations apply here.
4. **Image** is an optional field that lets you define a key image to associate with the event. This is achieved by selecting an image from the Image Assets app through the combo-box.
5. **Description** defines the descriptive text about the event which is seen when users navigate through to the event's detail page.
6. **Start** and **End** which define the Start and end date and time.
7. **Published** check-box defines whether the event is publicly visible on the website. Uncheck this instead of deleting it if the event is no longer needed. Note that past events are hidden from the public site and so don't need to be manually unpublished.
