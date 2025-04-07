# Prep
## Setup
+ Get my Debian environment setup on the laptop and get key packages
	+ Obsidian
	+ dev tools (IDEs/vim/emacs?)
	+ firefox
+ Customize the laptop, gotta look fresh
+ Research front end and back end tech we might use. Install them
## Supplies
+ HDMI cables
+ Expo markers
+ Headphones
+ Keyboard and mouse??
+ Previous year's shirt
+ Laptop and chargers
+ Snacks?
+ Notebook with pens
+ Sticky Notes
# Project Ideas
## Theme
**Financial Awareness**
## Our idea
We ended up settling on a new way to get money back from your friends GitBack. The idea here is to be able to create groups with your friends and others where you can request money. It will work far better than something like venmo requests because you can send batch requests and also accrue interest. GitBack will help by sending constant reminders to make sure you get your money back.
## Requirements
+ Login Authentication
+ Payments
+ Database holding all the goodies
# Process
## Initialization
It is the first night of the hack-a-thon and I am just setting up our tech stack for the next few days. It will use:
+ Next.js
+ Express.js
+ Render for postgres hosting
+ firebase?
[Setting up Next front end](https://nextjs.org/docs/app/getting-started/installation)
[Setting up an Express Server](https://www.geeksforgeeks.org/steps-to-create-an-express-js-application/)
[Setting up firebase](https://permify.co/post/firebase-authentication-nodejs/#step-1-setting-up-your-firebase-project)

[The github repo](https://github.com/1ando/GetBack)
## Code
After spending Friday initializing everything, Saturday would be coding day. This day is incredibly important for our success.

I started by working on the login Authentication.
[Firebase Authentication](https://permify.co/post/firebase-authentication-nodejs/)

Next I added the firestore implementation to the back-end. This involved creating the firestore database and making the basic schema we would be following.

I then worked on adding the following functionalities to the app:
+ Adding/Removing friends
+ Creating/Adding people to/Removing groups
+ Creating/Changing user settings

Finally I managed the middleware in the Next front-end so that content from the back-end could be loaded on the front-end. This involved managing cookies and creating get/post requests on the front-end to interact with the API created earlier.
# Contributions
I ended up building the login authentication, the firestore bucket for user data, and multiple back-end endpoints for the project.
# Failure
We gave up. Unfortunately, we spent too much time searching for geocaches and messing around. I stayed up until about 7 a.m. Saturday night/Sunday morning, but it was simply not enough with the progress we lacked on the front-end. We had to drop out of the event to save some embarrassment.
# Lessons learned
+ How to do firebase login authentication
+ How to set up and use a firestore database
+ If you want to win, full commit and not do the damn geocaches
+ Sleep is sacred
