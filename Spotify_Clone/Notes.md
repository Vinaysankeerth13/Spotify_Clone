**I am writing this to document the errors I got on the way and how I resolved them**

- All HTML and CSS was smooth.

- The first error I encountered was with spliting of songs, which was a very stupid mistake as it was just a parenthesis at a wrong place.

- Encountered an error with the getting the songs and trying to format them like 

from this :
http://127.0.0.1:3000/Spotify_Clone/Songs/Adavi%20Gusagusalu.mp3

to this : 
Adavi Gusagusalu 

it seems that the song name was not a string so I has to convert the type of song to string before trying to manupulate it. 

even later in the code encountered this problem as i was trying to code the play pause button and its interaction. But it was easy to resolve this time.

- While selecting a song from the list and playing it the code kept pointing to a diffrent URL like 

it was pointing to: 
http://127.0.0.1:3000/Spotify_Clone/Adavi%20Gusagusalu.mp3

while it had to point to:
http://127.0.0.1:3000/Spotify_Clone/Songs/Adavi%20Gusagusalu.mp3

It took me a lot of time to format all the songs and then get this thing to work but this will not be the case generally as we will be getting the songs using a external API call to the back-end, but since here we don't have that I used a local server. 

- When I was trying to preload a song as the first song of the list that plays whenever you first open the website I encountered this error 

http://127.0.0.1:3000/Spotify_Clone/Songs/Adavi%20Gusagusalu.mp3.mp3 not found, if we observe the .mp3 is showing up twice so we are not able to access the file. 

so to solve it i included a if case where if the name of the song ends with .mp3 we don't append .mp3 else we shall append it. 

- I encountered a git rebase error

