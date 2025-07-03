# Introduction
In an effort to put my creations out to the internet, I set my eyes on reviving the SongGuessr project that began slightly less than a year ago. The goal was to give the project a desperately needed glow-up. When bringing the project back from the graveyard, many issues came to light.
# Issues
## Efficiency
Hosting on AWS or my Raspberry Pi was impossible. The two API restriction from the hack-a-thon caused massive issues. We pulled enormous text files straight from the data dumps of the Music Brainz database which made loading into memory a problem.
## Accuracy
The gap from Artist -> Country worked well enough for a demo, but did not work well in practice. The main issue is that after choosing an artist, SongGuessr would search the artist by name in Spotify. Spoiler: many artists are not on Spotify or have a similar name to someone else. This gave many false positives in our system.
## Lack of Features
The core game play loop worked. However, nothing else did. There was no Spotify login and no leaderboard. These features were planned originally. We just did not have the time over our first weekend of development.
## Deprecation of Features
Spotify removed preview URLs from their API between this update and the project beginning. We needed an alternative for playing the music.
# Plans for Improvement
## Efficiency
The game would move to the API version of the Music Brainz database instead of using the data dumps. This saved countless amounts of RAM and storage. It did create a new issue. How would we get the necessary information? Some basic reading of the API docs showed how to pull artists by country.
## Accuracy
After having obtained the artist information from the previous step, we could search more information about the artist. In that information, we could find related links for that artist, including Spotify. This took multiple attempts due to most artists in the database having Spotify, but it worked well enough. 

In this process, #MongoDB became useful for storing Artists and their songs for later use. Efficiency took a bump here as well.
## Lack of Features
With MongoDB now set up, we could add leaderboard functionality for the users. A need for Spotify premium for the Web Player meant the leaderboard could also be attached to a user ID.
## Deprecation of Features
Sadly, song previews got removed. As a replacement, we added Web Player integration so that the browser could act just like a Spotify app on a phone or desktop.
# The Road Block
After completing all of these steps, Spotify released devastating news. Spotify would no longer allow for any apps to leave development mode without their explicit permission. Permission that would only be granted with 200,000 monthly active users. So, SongGuessr came to an end. I can still enjoy and have fun. The public will never get to enjoy it though. It was quite a sad realization that my project will no longer be able to see the light of day. Oh well, on to the next project.