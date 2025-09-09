# The Original Idea
When I first started this project, I planed to use a [Raspberry Pi Pico W](https://www.adafruit.com/product/5526) to interface with a Rust back-end. The end result would be a relatively small device that isn't my phone where I could track my workouts.

After researching and attempting to make the hardware portion work, I gave up for the time being so that I could work on getting the back-end working properly and adding a web interface. It's probably more usable for the time being anyway. While adding the web front-end, I got some inspiration from a little journal I bought at Barnes and Nobles.
# The Inspiration
Throughout college, I had stretches where of inspiration where I would actually commit to going to the LSU UREC. As almost anyone knows, it is very easy to start, but very difficult to keep it going. I felt this heavily. The main reason for this constant struggle came from semester to semester inconsistencies with my schedule. Balancing work, school, and hobbies can be difficult depending on the semester.

Well now that I am unemployed, that all changed. I can wake up anytime, go to the gym at any time, and there are no issues. Unemployment really is great (this is a joke). Anyway, I've been going strong for a few months at this point.

My memory is quite bad at remembering the weights I had previously lifted. So, I bought the [Body Minder Journal](https://memoryminder.com/bodyminder/) to help me track this. To help me learn Rust and keep my general skills up while I continue my job search.
# The app
The app is built with:
+ React
+ Rust
+ MongoDB
+ Firebase Authentication
I really shouldn't need to elaborate more about this because the app really is quite simple. Right now it can be used to store the workouts. When I decide to build this further, it will allow more elaborate data presentations and analysis. I wanted to get it online quickly so that I can start using it immediately.
![Gym Buddy Form](/assets/img/GymTrack/GymBuddyForm.png)
# Current Functionality
+ Sign in with Github using Firebase authentication
+ Log sets and reps for different exercises using MongoDB
+ Load in previous days of logs
# Future Plans
+ Data Visualizations on the web interface
+ Get into embedded programming by making a small device to interact with the web server
