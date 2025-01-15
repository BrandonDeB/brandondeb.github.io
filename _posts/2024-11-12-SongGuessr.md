---
tags:
  - hackathon
  - react
  - python
  - flask
---
I've been wanting to write some posts for this site for a while so let me take it back to 11/1/24-11/3/24 when I participated in a Hackathon. The event was put on by the Society for Asian Engineers and Scientists chapter at LSU. While neither me nor my two teammates Landon and Koby are Asian, we still aimed to participate and win.

In order to ensure a great idea on Friday when the event first started, I did not go get frinks the night after Halloween, but rather brainstormed ideas with my team instead. Our idea had to be related to international travel or encourage people to explore other cultures. To satisfy the prompt and also have fun making the project, our group PPPPHMOOC (please please please please hire me out of college) decided to make a Geoguessr-esque game, but with locating the origin of songs again. The idea was that this style of game could be integrated with Spotify to allow users to find new unique music they liekly had never heard before.

On that Friday night, I spent time researching possible ways to make it happen. My first discovery was [this npm package](https://www.npmjs.com/package/globe.gl) that would allow us to have a cool interactive map without doing insane amount of work. Then I discovered the [MusicBrainz API](https://musicbrainz.org/) for finding artist locations. The main issue with MusicBrainz, however, we were planning to use Spotify for the one API the event allowed us. Luckily, I managed to find the data dumps that MusicBrainz regularly publishes.

The next morning, we began work on the actual project. My first task was to get the interactive map working. Using the documentation, I managed to complete the implementation of the map. Next, I switched over to gathering all the data needed for the project. Normally, this would be trivial because MusicBrainz API had search functions to find artists from varying locations. Using the data dumps meant finding this information manually. After writing a scraper to find the coutnries for hundred of thousands of artists, I output only the relevant data making the filesizes thankfully much smaller.

All the while, my teammates worked on the visual design of the site and the backend. The biggest hurdle for the project was connecting the user authentication for Spotify into our app. Unfortunately, we were unable to complete this aspect so we were only left with the main game itself.
The presentation I thought went well with the judges asking to keep playing, but we did not finish very well in the event. The lack of Spotify integration hurt our points in the impact category. I am still happy with the placement and had a good time at the event.

## Some Pictures!
![PPPPHMOOC at work](/assets/img/Songuessr/at_table.jpg "At a table")
![Everyone after the event](/assets/img/Songuessr/group.jpg "Group picture of everyone")
![PPPPHMOOC presenting](/assets/img/Songuessr/Presenting.jpg "PPPPHMOOC presenting Songguessr")
