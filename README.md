# Chromia maps

The note data of the maps that come with Chromia's Roblox place. The place
keeps each map's name, mapper and difficulty in its `Maps` module; its server
downloads the rest from here when it starts (the song id, the notes, and from
them the note count and length):

    https://raw.githubusercontent.com/iloverhythia/maps/main/maps/<file>.txt

A file is a map in Sound Space's format: `audio id,x|y|ms,x|y|ms,...`
(x and y from 0 to 2, across and down the grid; ms is when the note is hit).
The audio id at the start is the Roblox audio the place plays for the map.

To add a map: put its file in `maps/`, then add a block for it in the place's
`Maps` module with its details and `url = BASE .. "<file>.txt"`.
