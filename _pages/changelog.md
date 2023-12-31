---
layout: page
title: What's New
include_in_header: true
---

# Changelog
Here you can view a changelog and version history for **WristCheck**. Got some suggestions for features you’d like to see in a future update? Please feel free to mention in an app review via Apple or Google, drop me an email or @ me on Twitter _(or whatever it's called this week)!_

<br>

### `Latest`
# **Version 1.7.1**
Another self-contained, _big_ release, and one that I'm really proud of! When I built **WristCheck** I initially wanted to be able to use data to really _understand_ my collection and how I interacted with that. The _Wear Charts_ were the first manifestation of this, however they were quite basic, only showing individual watches with counts which could be filtered by a combination of month and year...
With version 1.7.1 though I've attempted to supercharge that! You can now see the charts over alternative time periods (such as last 30 or 90 days), have additional options to group the results (by watch, by manufacturer, by category or by movement type!) and you can filter the results to include or exclude sold and archived watches, or to only show specific movement types or watch categories!

#### What's New
- Update to Wear Chart screen to include new filter and grouping options.
- Group charts by watch, manufacturer, category or movement type.
- Filter chart by new time periods, by movement type or by category.
- Include or exclude Sold and Archived watches from the reports.

#### Bug Fixes
- The new implementation of the Wear Charts will extend past the bottom of the screen and become scrollable if there are a lot of records returned. This fixes an old bug where if you had ~30 watches being displayed, the names of every second chart line disappeared.
- In line with the above, the chart Screenshot functionality has been updated to automatically capture the full size of the chart and any current filter information when the button is pressed.

<br>

# **Version 1.6.4**
This release includes a few small improvements and bug fixes which didn't feel like they warranted a large version bump. Behind the scenes updates include implementation of improved crash logging and analytics to help me to make the app _better,_ as well as a new pre-order status to provide a countdown to a watches target release/delivery date.

#### What's New
- Updated notification code to work with the latest versions of Android and iOS.
- New Pre-Order status to allow a countdown to watch release.
- Option added to do a bulk export of all watch images, making it easier to move to a new device.
- Implemented Crashlytics logging and Firebase Analytics to help to quickly address performance issues and to better understand app usage to guide future updates.

#### Bug Fixes
- Fixed an old bug where the in-app version history wouldn't fully scroll to the bottom.
- Slight adjustment to notification code to keep the notification at the scheduled time during daylight savings time changes.

<br>

# **Version 1.6.1**
In version 1.6 I have focused on improving the add/view/edit watch user interface, to (hopefully) make it more intuitive to use, and easier to find the details you want quickly!

Additionally, this release includes new data points that you can save for each watch, including: category, movement type, and purchase and sale information (such as date, price and who the watch was bought from/sold to).

Of course more data also means more analysis, so the app can now also provide a 'cost per wear' value for each watch, charts showing the movement types and watch categories that make up your collection as well as calculations of collection spend amongst others.

#### What's New
- UI overhaul of the add/view/edit watch pages
- Capture more watch details such as category and movement types
- Capture watch value data such as purchase and sale dates, prices and who the watch was purchased from/sold to
- Additional information added to the collection stats section, including additional charts and data analysis

#### Bug Fixes
- The way database backup works has been changed to avoid a crash issue on iOS - now rather than the app attempting to write a copy of the database to a new location, it pushes a copy to the platforms 'share' function, allowing you to send the database copy wherever you like quickly (I'd recommend sending to iCloud/Google Drive or similar every so often!).

<br>
# **Version 1.5.1**
In version 1.5 the main update is a change to the user interface of the main watch box view. The page now shows watch images (if you've added them!), adds various options to change the display order of the watches and lets you choose between the original list view, or a grid view with larger images.
It also makes access to search more prominent and makes it easier to switch between your various 'watch boxes' (e.g. your wishlist or sold watches)

#### What's New
- UI overhaul of the main watch box
- Watch images now show in watch box view
- Quicker access to search
- Choose the display order of your collection
- Choose a list or grid view for the UI
- Updates to software libraries and OS target levels

#### Bug Fixes
- Includes a fix to the original v1.5 which caused overlapping text on the grid view when on a smaller screened device.

<br>

### **Version 1.4.1**
This update focuses on making me rich... wait, sorry! It focuses on letting users remove ads from the app with a quick and simple in-app payment. I rely on the ad income to help me cover the development costs of the app (sadly it's not free!) but in this release have added a way to remove these, and allowed the user to pick the price they pay to do so.

#### What's New
- WristCheck Pro added!
- Remove Ads with an in-app purchase
- Pick chart default order options

#### Bug Fixes
-  Bug fix related to saving images with special characters in the watch name

<br>

### **Version 1.3**
I love looking at the back of some of my watches almost as much as I love looking at their dials! So in this update I've added the ability to capture a second picture for each watch - nobody is forcing you to use this for the case back of course, but that's why I put it in there!
The update also adds the ability to upload the watch images at the same time you add the watch record to the app, rather than having to go in and do it as a second action (which I'm sure you'll agree is an improvement!).
To improve the chart experience I've also included the ability to set defaults for the chart view (so you can have it always show the current year, current month, previous month or all time stats).
Lastly I've included logic that will prompt to leave a rating or review after a period of time using the app - please consider using this as ratings really help with app visibility!

#### What's New
- Caseback images - add a second photo to each watch
- Add images when creating new watch records
- Chart Preferences - set default filters and chart types
- Added 'review app' prompt

#### Bug Fixes and minor improvements
-  Refactor of code for better image management
-  Auto Capialise Watch Names
-  Help text improvements for watch wear history view
-  Improved placement of image picker (Gallery/Camera) option

<br>

### **Version 1.2**
A relatively small release, v1.2 introduces small ads throughout the app - I've tried to keep these as unobtrusive as possible - most are small banner ads, with some pages with more whitespace showing slightly larger banners.

#### What's New
- Implemented unobtrusive banner ads throughout the app
- Added a button to save and share screenshots directly from the wear chart screeen

#### Bug Fixes and minor improvements
-  Fixed permission prompt issue for Android notifications.


<br>

### **Version 1.1**
In the first major update to WristCheck a _'what's new'_ pop-up has been included, that displays whenever the app is updated to advise of any new features - and to make use of it this release also includes an option to backup and restore the app database, as well as introducing the option to setup a helpful daily reminder to track what watch you're wearing.

#### What's New
- Implemented a 'what's new' pop-up that shows when the app version updates
- Backup & Restore the watch database
- Set up daily wear reminders

#### Bug Fixes and minor improvements
-  Reference number field added to watch model


<br>
________
<br>

### `Initial Release`
# **Version 1.0**
Welcome to WristCheck!
I've built this app as a digital watch box companion - you can use it to track the watches you own and how often you're wearing them, as well as to track a wish list of watches that you'd like to purchase in the future.

#### Main Features
- Create a database of your watches
- Keep a wish list of watches you'd like to buy, and track watches sold
- Track when you wear your Watches
- Draw graphs to show what watches you're wearing most over time
<br>
