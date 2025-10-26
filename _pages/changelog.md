---
layout: page
title: What's New
include_in_header: true
---

# Change log
Here you can view a change log and version history for **WristTrack** - I try to keep this updated whenever I release a new version, with a little commentary around the changes made and their inspiration. You can always find the latest summarised release notes within the app in the 'About App' section, found within the main sidebar.

 Got some suggestions for features, bug fixes or improvements you’d like to see in a future update? Please feel free to mention in an app review via Apple or Google, [drop me an email](mailto:feedback@wristtrack.app) or message me on [Instagram](https://www.instagram.com/wristtrack.app/)!

<br>

### `Latest`

# **Version 1.15.1**
This latest version is long overdue - partly because I started working on some new features that turned out to be a little _too big_ (watch out for that in the next release hopefully!), but also because this release required quite a bit of work to get the app builds working when targeting the latest versions of Android and iOS (to keep the app in the stores these updates are required every year). This process often grows arms and legs, as updating one dependency then requires additional change and testing to keep things working - this years update proved to be a bit of a headache!

Due to these, whilst this update took a while to deliver it's also relatively small, but hopefully useful! The first major update is a change to the watch images - instead of the previous front / back images, there's now a three image gallery for each watch, with a much nicer UI:
If no image is in a space tapping on it brings up the image picker. If an image does exist, the image is enlarged to bring up a larger gallery for the watch.
In the gallery images can be replaced or deleted with a long press (can you believe that until now there was no way to delete an image in the app, only to replace it!).

Another update in this release is a new 'delete watch' button - of all the messages I receive the most common question has been "how do I delete a watch I've added in error?".
Until now, this process was to edit the watch, change it's status to 'Archived' and then delete from the Archive... long winded, and not super obvious! Now, if you edit the watch a 'delete' button appears, and when pressed a confirmation dialog appears asking the user if they want to continue.
The watch is still 'soft deleted' first, by moving it to the Archive (so it can be restored to the collection easily), but hopefully this is a much nicer user experience!

Finally, there are now three new currencies available to select (as below) - as always, if there's something missing feel free to reach out and ask, always happy to add these in :)

#### What's New
- Improved watch image gallery and ability to save third picture, as well as ability to delete pictures
- Improved UX flow for deleting a watch
- New currencies added: Norwegian Krone, Thai Baht & Czeck Koruna

#### Improvements
- Updates to the calendar view to ensure all appropriate watch statuses display
- Updates to the CSV data extract options to include all the recently added
- Updates to numerous libraries to support latest OS versions

<br>

# **Version 1.14.0**
This update is more evolution than revolution - and as always heavily influenced by comments in reviews and messages I've received from app users. Firstly, there was a suggestion of laying out the key dates tracked in a timeline - a way to see what watches had been bought and sold and when, along with other dates like warranty expiries and tracked services. I loved this idea, so in the 'More' section of the app I've implemented a TimeLine view, this shows any dates tracked in the app, with the ability to toggle on or off different types to change the view.
Another request I received related to the ability to add watch names in Russian or other Cyrillic alphabets, so the validation rules have been updated to allow watch names using these characters to be saved (and a huge 'thank you' to Egor for providing some sample watch information to help me test this out!).
Other changes are smaller - such as adding some text with watch info to the gallery view (which can be toggled on or off with a tap) and adding additional information to the Pro data section.

#### What's New
- New TimeLine view Added
- Updated validation rules to support Cyrillic alphabet
- Polish Zloty added to currency options
- Watch details added to Gallery View
- (Pro) Toggle added to hide monetary values from the cost per wear charts
- (Pro) Ability to track date complication added to the Pro data section, along with associated charts
- (Pro) Ability to save watch winder settings added

#### Improvements
- Background colour added to watch box and selection drop downs to improve visibility
- 'Not Entered' value removed from case material charts
- 'All' option added to the Gallery view (showing all non-archived watches).
- (Pro) 'Nerd Data' renamed to 'Pro Data' on the Watch detail view

#### Bug fixes
- Fixed an issue where some collection charts would fail to load where null values were encountered
<br>

# **Version 1.13.0**
I recently visited my first watch group meetup - a Redbar Glasgow event where representatives of Christopher Ward were on hand to show off their range of watches (for anyone who follows my Instagram account, that's where I fell in love with the 38mm Twelve in peach that I later went on to purchase...). During the event I was chatting with some people about our collections and I instinctively pulled out the app to show them some stats... and realised that it was _useless_ for the purpose of _showing off your collection_. I honestly thought nothing of it and mumbled an apology before loading up Google Photos and searching for the watch I wanted to show them.

A few weeks later though I got a suggestion from a user (I've said it so many times, but I really do listen to these!) who said "why not add a gallery view to quickly show off your watch collection" and that prior event sprang back to mind! Could I do that? Would the images saved be high enough quality to show full screen (I purposely crop and compress images in the app when taken, as the photos are meant to act as thumbnails)... would this make sense from in the UI?

So I went away and did what I often do and started prototyping on a safe code branch... and you know what... the answer to the above questions were all _'yes!'_

So the main update in this release is a new watch gallery view - you can look at all the watches in your collection, or use variations on existing filters to look at your favourites, sold watches, wishlist, or other options where you may have saved pictures in the app! (and of course I'll use these foundations to add to future improvements too!).

Additionally I continued to extend the 'nerd stats' section available to Pro users to add some more data points - this time adding a field for water resistance ratings, and another for case materials... and of course you can also see aggregate charts for these in the collection stats pages, or use them to filter the wear charts!

#### What's New
- Gallery View
- Additional 'Nerd' data and charts for Pro users - Water Resistance and Case Material

#### Improvements
- Any feedback email triggered from the app adds the app version and platform to the email subject
- Keyboard triggers updated for iOS users to ensure that they can include decimals (where appropriate) in case dimensions

#### Bug fixes
- Pie Charts now work for all Pro related chart filters (case dimensions etc)
- Fixed an issue where Android 15 users were unable to save watch images
- Updated daily reminder text to amend _WristCheck_ to _WristTrack_
- Defensive code added to help reduce Google Admob related soft crashes



<br>

# **Version 1.12.1**
I started this release with some good intentions - I really wanted to release a new feature, _Wrist Recap_, before the end of 2024, to act similar to _'Spotify Wrapped'_, giving users a summary of their collection and wearing habits over the course of the year... however the more I looked at it, the _bigger_ it got! Which was proving detrimental to getting it finished and moving onto other, long promised work... and past the point where it would arrive in 2024!

Instead I got it to a point where the foundations were in place - it will let you pick a year from any with data, create some data sets based on this and structure the data for easy access and handle things like empty values... it only shows changes in collections size, overall wear count and the top three watches worn in a year though - but the _potential_ is there! So in this release it's got a _'BETA'_ tag on it as it's just a starting point for something more to come. I considered turning it off, but thought releasing it would gather more input and feedback (and if you have any, please reach out!)

This let me then move onto something I've been promising for a while - _more data!_ I've limited this to Pro users, as a way of adding additional value to the Pro upgrade and started off with case dimensions (diameter, thickness, lug to lug and lug width). These can all now be added on the new 'Nerd' tab Pro users will see on the watch pages... and of course _more data_ means _more charts_, so within Collection Stats each data point has it's own chart summarising your collection, and within Wear Stats you can now group your wear stats by these (which case size do you wear most?).
This builds on the foundations I laid out in v1.11, and is the start of a wider push to expand the data in the app. My intention is to add a few points in each release going forward.

Next up, a couple of new currencies available as options (both requested by users, so please reach out if you'd like to see more) - Swiss Francs (CHF) and Hungarian Forint (HUF). It was nice to revisit this and see how simple I'd kept the code for currency, as adding these was super easy... thanks past me!

Another pro only feature is the new Moon Phase calculator on the Time Setting tab - for non-pro users I show an ad at the bottom of this screen, but for Pro users there was lots of unused space, so filling it with a representation of the current moon phase made sense, and is hopefully useful for those with this complication (I _love_ the idea of a moon phase complication, but find most options to _dressy_ for me!).

Finally, I've made it easier to get in touch with me from within the app by adding an email link directly in the sidebar!


#### What's New
- Wrist Recap (BETA).
- New Case Dimension data points, charts and filters.
- _'Wear this Watch today'_ button dynamically changes to _'Worn Today'_ once pressed.
- Added Swiss Franc and Hungarian Forint to the currency options.
- Moon Phase calculator added to the Time Setting page for Pro users.
- Developer feedback email link added to the app sidebar.

#### Known Issues
- There is now a bug with Android 15 preventing images from cropping successfully - a fix has been identified and included in v1.13 which is due _imminently!_

<br>

# **Version 1.11.0**
A relatively light update, with a lot of the change incremental and behind the scenes, with many small changes made based on user feedback. A key example being the new 'Retired' status - perfect for those older watches you may have lying around that don't get worn anymore, but that you'll also never let go of! Retired watches don't show in the main collection, but can be filtered from the main view in the same was as Wishlist or Sold watches.

In addition, at a user request, I've added a 'Since last Purchase' filter option to the Wear charts - you can now see how you've been wearing your watches since you last added a new one to the collection - just how strong is that _honeymoon pull!_

#### What's New
- Added a new 'Retired' status for Watches.
- The first day of the week is now manually selectable in settings for all calendar views.
- 'Since last Purchase' filter added to the Wear Charts.
- Added manual selection of Light/Dark theme, rather than relying on system default only.
- When tracking wear directly from the calendar view, the searchable watch picker dropdown now shows watches in the same order as the watchbox view preference.
- Updated 'What's New' pop-up, giving more space and a cleaner look.
- [Hidden] Refactor of the Watch detail page in advance of upcoming changes to add more data.

#### Bug Fixes
- The Cost per Wear chart now resizes based on the size of the collection, to ensure all entries are visible.

<br>

# **Version 1.10.0**
I had planned a larger release for v1.10, since its the 10th major release of the app (time flies!), but I also got a new laptop recently which meant migrating all the parts of my dev setup that aren't backed up in Github (such as API and signing keys), so decided to focus on one main feature that I've wanted to add for a while and make available to everyone - a new network synchronised clock!

There's now a new tab on the main page labelled 'time' which opens up a clock displaying the current time - it starts of based on the device system time, but quickly gets responses from network time servers (and will continue to improve accuracy as more servers respond) to show the most accurate time possible. I've also implemented an optional audible countdown of the last few seconds each minute (with a larger 'chime' when the clock hits "00") to help accurate time setting. (As an aside, I find it a little amusing that despite mechanical watches often only being accurate to a few seconds a day, I still *really want* to make sure they're accurate when I set them!)

When I added the calendar view in v1.8 I was also asked if I could provide an option to make it the main screen (as some users like to look at the calendar and quickly see if they've missed any dates), so with the addition of the time page I was happy to oblige, and there's now an 'app preferences' screen within Settings to allow selection of either the Collection, Calendar or Time screens as the app home screen.
Whilst making this settings page I also included the option to amend the collection ordering and List / Grid setting here too (previously this was only available in the pop-up screen found on the collection view, but no harm in having these options in two places!).

Finally, I made a few under the hood updates - Google notified me that I needed to update the app to target to the current Android version (ahead of the new version coming out) as well as to use the latest version of the Play Billing library (which for me is packaged as part of the RevenueCat SDK I utilise for in-app billing) - these changes need to be made once a year to keep up to date with the latest Android standards, so with these updates made I can look forward to doing the same again next summer (although similar updates for Apple are likely required later in the year!). Since I'm on a new laptop I also updated the Flutter SDK version and had to make some smaller updates to the app build scripts... all boring tech stuff!

Oh, and I had a couple of references to WristCheck that I found and updated to WristTrack!

So that's it for v1.10 - as always feedback is appreciated!

#### What's New
- New Time page - get the accurate time (with optional audible countdown) for setting your watches.
- Home page selection - choose whether the app should open to your collection, calendar or clock.
- Tidied up some leftover references to 'WristCheck'.
- Under the hood updates to use the latest versions of the Flutter development SDK and RevenueCat libraries, as well as incrementing the Android SDK build target (the latter two changes are required to keep the app in line with Android policies).

<br>

# **Version 1.9.1**
A super quick, but important update - version 1.9.1 updates the app name from *WristCheck* to **WristTrack**.

When I set up the app I naively didn't think to check if the name was already being used elsewhere, so was surprised to find _WristCheck_ is a registered trademark - full credit to the team at [WristCheck.com](https://www.wristcheck.com) (the holders of the trademark) though, they were excellent about it and I was able to get an update together for the app within around a week.

I'm sure I've missed a reference or two to 'WristCheck' within the app, but I'll get those tidied up in the next release (which is just around the corner!) - for now though, I hope you all enjoy **WristTrack** as much as you did when it had it's old name!

#### What's New
- An app rename (along with associated update to this website!) from _WristCheck_ to _**WristTrack**_

<br>

# **Version 1.9.0**
A relatively big update this time, with some nice new additions and the first 'WristCheck Pro' feature drops - to date all functionality has been free to everyone, and it's important to me that the app provides value to everyone (I didn't set out to make money, I set out to make an app for fellow watch nerds!) but I think the app has now reached the point where it's got a really solid set of core features (watch data tracking, wear tracking and charts, a visual representation of what you've worn via the calendar etc) so felt it was time to add a few wee extras for the extra nerdy amongst us!

But first up, I wanted to include some more features that improve the app experience for everyone...

First, the app logo has been added to the sidebar - I know this is a really minor update, but I think it really improves the whole sidebar! This goes hand in hand with some slight adjustments to add a new 'App Data' menu item, to bring together the existing Backup/Restore features and the new **CSV Extracts** option.

This allows you to export your data in two forms, either a simple list of each watch with all their data and a consolidated wear count (useful if you need a quick list for insurance purposes perhaps?) or a second more complex option, that has one line for every recorded wear (so multiple lines per watch) - perfect if you want to do your own data analysis!

Next up, I've also replaced the old date-list view with a calendar view, showing wear dates, servicing and warranty dates on a per-watch basis. From here you can quickly review, add and delete wear records for the chosen watch.

So, onto those 'WristCheck Pro' features - as mentioned, I don't do this to make money (I'm _not even close_ to the point I could claim to earn minimum wage from my wee apps!), but I did want to start adding some little extras for supporters, and wanted to focus on exactly that - **extras** - fun wee additions that just add a bit more value for the _real nerds_ among us!

First up - and something I've had a few requests for - the ability to set a second daily reminder. Quite a few people wear a work watch and then swap over in the evening, so now they can get reminded to log into the app twice a day to track what they're wearing.

Then, last but by no means least, I've added some per-watch graphs (currently accessed via a link from the watch page, but I'll add something to the 'stats' page in the next drop) - initially two options are available - a breakdown of wears by month, and another of wears by weekday. Not going to lie, I _love_ wee graphs so this is my favourite addition and works well! I'm planning to further refine these in future releases and will probably add more - as always please feel free to drop me a note with any ideas or suggestions.

#### What's New
- The WristCheck logo has been added in the sidebar menu, along with a slight menu re-design.
- The Calendar view is now extended to give calendar breakdowns for individual watches - quickly review, add or delete wear dates.
- CSV data extracts - generate simple (one line per watch) or complex (one line per wear record) CSV extracts, to quickly summarise your collection or to draw your own charts!
- (Pro) WristCheck Pro users can now set a second daily reminder.
- (Pro) New watch data charts are available to Pro users, showing a breakdown of wearing habits for individual watches, by weekday or by month.

<br>

# **Version 1.8.0**
When I first built WristCheck I was relatively new to watch collecting, having recently purchased my first mechanical watch... I was also clearly quite naive as I thought a schedule of when services were due would be a headline feature of the app! Instead, I got quite a bit of feedback that, whilst it's useful to know when servicing is due per manufacturers suggestions, many owners only get their watches serviced at the point where they notice a drop in accuracy.
I've also never been happy with the lack of visualisation of how your wear tracking is going, which was visible as a big list of dates per watch... so this fix hopefully addresses this with the addition of a new **Calendar View**.
From the main landing page, this replaces the third page tab, and populates a calendar quickly highlighting each day where a watch wear has been recorded, as well as showing upcoming service due dates (if tracked) and **warranty expiry dates.**
Speaking of which - you can now also add a warranty expiry date to your watches!

But what about the old servicing view? It wasn't useless, but definitely was a _secondary feature_ (i.e. not necessarily a primary use case for most) of the app and therefore rather than getting rid of it, I've simply moved it to a more appropriate place.
On the calendar view there's a small circular button that changes from a month/day calendar view to the old servicing view, however it's now been tidied up and includes tabs along the top to switch between a service schedule and a warranty end schedule.

With this release I think I'm now happy with the primary features of the app, so going forward the next few updates will all be about just making things _better_. As always, if you have any feedback please feel free to drop an email to [feedback@wristcheck.app](mailto:feedback@wristcheck.app) or write an app review on your favourite app store - user input genuinely does help me continue to improve the app!

#### What's New
- New Calendar view (replacing original Servicing schedule as a main tab), visualising all wear data.
- Ability to see a list of all watches worn on a selected date, as well as other scheduled events such as service due dates.
- Ability to add wear records directly to the calendar.
- New warranty expiry date field added to the Watch model.
- Updated Schedule view, allowing a user to view a chronological service due schedule or a warranty expiry schedule.
- Website link (www.wristcheck.app) added to the About App info, along with some smaller cosmetic updates here.

#### Bug Fixes
- Updated the calculation algorithm for the 'cost per wear' value - this now takes into account any returned value when a watch is sold.

<br>

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
