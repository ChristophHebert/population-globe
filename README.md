# Population Globe

Population globe is a digital rendering of the earth using latitudes and longitudes of densely populated cities. The goal is to inspire a people centric perspective of the world's geography.

View working result [on my website](https://christophhebert.com/digital-globe/ "Homepage of ChristophHebert").

![rendering of globe using city locations](https://christophhebert.com/digital-globe/image.png "Population Globe")

City location data is pulled from DBpedia's [SPARQL interface](http://dbpedia.org/sparql) using the queries currently in the .txt files, and stored in the corresponding .json files.

Open index.html in a browser in a server-type environment (in other words, you have to using a local server like MAMP or actually have index.html and the corresponding .json files on a server in order for the send/recieveAjAX functions to work properly), and a globe should appear with buttons to rotate the rendering.
j
## ToDo:
- Use DBpedia links in json data to link each cities' dot to its corresponding Wikipedia page.
- Allow user to hold down rotation button for continuous rotation rather than furiously clicking.
- Allow user to click and drag for rotation.
- Add optional parameters for user to adjust population cutoff for cities.
- Highlight a random city for user discovery upon each new page load.
- Make rendering responsive to user's browser window and optimize for embedding into web pages. (Rendering is already responsive to changes of canvas size.)
- Consider accounting for geometry of how a real world viewer cannot necessarily see the entire 180 degree portion of a sphere. (Side effect: this would create the need for vertical adjustment of perspective in order to see all surface area in addition to existing horizontal rotation).
