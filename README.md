# Chromia maps

The note data of the maps that come with Chromia's Roblox place. The place
keeps each map's name, mapper, difficulty, song, note count and length in its
`Maps` module, and its server downloads the notes from here when it starts:

    https://raw.githubusercontent.com/iloverhythia/maps/main/maps/<file>.txt

A file is a map in Sound Space's format: `audio id,x|y|ms,x|y|ms,...`
(x and y from 0 to 2, across and down the grid; ms is when the note is hit).

To add a map: put its file in `maps/`, then add a block for it in the place's
`Maps` module with its details and `url = BASE .. "<file>.txt"`.
