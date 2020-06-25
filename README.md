**(6/24/2020) Group Buy Organizer being rewritten in new repository!**  What started as a project to learn about web frameworks is now being completely rewritten in Django, with plenty of more features and capabilities.  Once completed, it will be its own site online that anyone can use (domain TBA).  I expect to have it done sometime before the 2021 fireworks buying season.  Click the link below to follow along with my progress:

**[https://github.com/MarkMichon1/groupbuyorganizer2](https://github.com/MarkMichon1/groupbuyorganizer2)**

### Organize Group Buys Faster

**Group Buy Organizer** is a web application that helps manage wholesale group buys.  Remove a lot of the overhead
involved in coordinating purchases with users.

**User Features**
+ **Fast and flexible group buy system:**  No more back and forth between participants and the organizer.  Want to
change your order?  Just log in and make the changes.  They will instantly change the order for the organizer.
+ **Streamlined case-split system:** Splitting a case with others just got a lot easier.  Pledge how many items in the 
case you'd like to order, and other users can make pledges as well.  Once all of the items in the case gets accounted
for, only then it gets locked into the order.
+ **Multiple order views:**  Three different views of event orders are available for users.  The user overview view is 
a customized list showing the cases and items you've ordered, its subtotal as well as the event total.  The event 
summary view is a concise list for the organizer of how many cases to order.  The user breakdown view steps through one
item at a time, showing all of the users who bought cases of it, as well as all of the case splits for that item.
+ **Export to PDF:** All order pages include a button to export the list as a PDF to be downloaded.  Pages are stripped down and optimized, removing the navigation bar, forms, etc.  Only black and white is used on exported pages.

**Administrative Features**
+ **Complete control of the application:**  Expanded functionality added to edit virtually all aspects of group buys.
Change and remove items, add item categories, remove users from an event, promote others to admin rank, and more.
+ **Optional restriction of event information:** Prevent users from seeing the orders of others, as an optional feature.
+ **Decide who has access to your application:**  User registration can be disabled, and any users can be removed from 
the application with a single click of the mouse.

### Using Group Buy Organizer

**Initial Setup**
After the application is properly installed and running, create a user account.  The first account to register will be
given "root" access in the application, all other registrations will be "user" tier.  From there, all there is left to 
do is to setup categories, and to create an event.  Click the admin button on the top right, and click "Category 
Settings."  Create whatever product categories that will be used in your group buy.  From there, go to home and create
an event.  Thats it!

**General Use**
In order to use Group Buy Organizer you must register an account.  Once thats done, go ahead and log in.

This is the general flow of the program:  Using your price sheet/case list from the wholesaler you'll be purchasing 
from, if the items already haven't been added by someone else, add them to the event using the form at the top of the
page.  Once items are added, anyone is free to interact with them, whether you want to buy cases for yourself, or split
a case with some other people.  While the event is open, any user is free to add as many items, and to buy as many cases
or involve themselves in as many case splits as they want.

As the event comes to a close, an administrator will lock it (Event Settings).  This will lock in all transactions, and
no user can add, remove, or change their order.  Things become finalized at this point, and you can check out the totals
using any of the available event total buttons on the event screen or on the home screen.

### Installation:

Installation is simple.  You can either download the repository from this Github page, or via PyPI: `pip install 
group-buy-organizer`

In order for the PDF functionality to work, you must download a binary that the program will use to convert pages to 
PDF:
https://wkhtmltopdf.org/

Download and install on your server.  Go to "Application Settings" in the admin menu, and follow the instructions from
there as to how to properly link it.  The whole process only takes a couple minutes.

Once thats done, everything is good to go.

Libraries used:
- `flask`
- `flask-bcrypt`
- `flask-login`
- `flask-sqlalchemy`
- `flask-wtf`
- `pdfkit`

### License

MIT License

Copyright (c) 2019 - ∞ Mark Michon

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
