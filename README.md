# Population Globe

Population globe is a digital rendering of the earth using latitudes and longitudes of densely populated cities. The goal is to inspire a people centric perspective of the world's geography.

View working result [on my website](https://christophhebert.com/population-globe/ "Homepage of ChristophHebert").

![rendering of globe using city locations](https://christophhebert.com/digital-globe/image.png "Population Globe")

City location data is pulled from DBpedia's [SPARQL interface](http://dbpedia.org/sparql) using the queries currently in the .txt files, and stored in the corresponding .json files.

Open index.html in a browser in a server-type environment (in other words, you have to using a local server like MAMP or actually have index.html and the corresponding .json files on a server in order for the send/recieveAjAX functions to work properly), and a globe should appear with buttons to rotate the rendering.

## ToDo:
- Correlate perspectiveUnit to canvas width to distance along the equator so rotation rate feels natural.
- Use DBpedia links in json data to link each city's dot to its corresponding Wikipedia page.
- Add optional parameters for user to adjust population cutoff for cities.
- Highlight a random city for user discovery upon each new page load.
- Optimize for embedding into web pages as a widget of sorts.
- Consider accounting for geometry of how a real world viewer cannot necessarily see the entire 180 degree portion of a sphere.
- Implement vertical rotation in addition to horizontal.
