Auth
====

Short for "Authentication", Auth is where you manage user profiles, who can log in and what they can edit when they do.

Auth models
-----------

Auth contains two models, Groups and Users. The latter contains individual profiles for users with all their associated privileges, the former allows admins to assign privileges to defined groups. Users can then be added to those groups and inherit their privileges from them. Groups makes it very quick and easy to set up quite specific levels of privileges initially, and then apply those privileges in bulk quickly and easily.

Groups
------

1. Click Home > Auth > Groups
2. Here are listed all the groups that can be applied to user profiles.
3. To edit an existing group, click the group name.
4. To add a new group, click "Add group".
5. **Name** defines the tag that can later be applied to user profiles
6. **Permissions** defines what permissions a group has. The left column contains all the available permissions in the system, while the right contains all the permissions  assigned to the current group.
7. Individual permissions can be moved between the columns by selecting items and then clicking the arrow icons; or by double clicking an item.

Users
-----

1. Click Home > Auth > Users
2. Here are listed all the user profiles registered with the system.
3. Each user presents the following bits of meta, from left to right…
    1. Username (click here to view)
    2. Email address for this user
    3. First Name
    4. Last name
    5. Staff status (a tick here indicates that the user has access to the admin dashboard)
4. To edit an existing user, click the username.
5. To add a new user, click "Add user".

Adding a user
`````````````

Adding users is a two stage process. It's recommended that you undertake both in order to fully create a user profile in a single sitting, but this isn't strictly required…

1. Click Home > Auth > Users > Add user
2. **Username** is the name that a user uses to access the admin, must be 30 characters or fewer, consisting of letters, digits and @/./+/-/_ only.
3. **Password** and **Password confirmation** should be identical for verification purposes.
4. Click "Save and continue editing", the page will refresh with the second tier of options.
5. You will note that the username value previously filled in is reproduced here. The password will look broken - don't panic! It's not broken, it's encrypted so that other users can't abuse other user's passwords.
6. Personal info
    1. **First name**
    2. **Last name**
    3. **Email address** for ease access and support.
7. Permissions
    1. **Active** checkbox designates whether this user should be treated as active. Unselect this instead of deleting accounts.
    2. **Staff status** checkbox designates whether the user can log into the admin site.
    3. **Superuser status** checkbox gives you super powers! No, seriously it designates that this user has all permissions without explicitly assigning them.
    4. **Groups** defines whether the user belongs to a group, inheriting that group's permissions.
    5. **User permissions** defines what permissions a user has in addition to inherited group permissions. The left column contains all the available permissions in the system, while the right contains all the permissions  assigned to the current user.
    6. Individual permissions can be moved between the columns by selecting items and then clicking the arrow icons; or by double clicking an item.
8. Important dates
    1. **Last login** denotes the date and time of this users last use of the CMS.
    2. **Date joined** denotes the creation date of the users profile.
    3. Both these fields can be edited, but are included largely for reference purposes.

Editing a user
``````````````

1. Click Home > Auth > Users > [username]
2. has the effect of dropping you directly into the second of the two stages, point 5. under "Adding a user" above.
