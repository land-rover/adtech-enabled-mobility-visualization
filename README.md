# Visualizing Geospatial Time Series Data

Publicly-available individual-level mobility data is an artifact of the ubiquitous cell phone.  

Because the data is enormous, any profitable study of it must begin with a visualization.

My favorite visualization approach comes from a company called [Tectonix](https://www.tectonix.com/).

To appreciate their approach, consider an interest in spreader events.

During a spreader event, a group of people gathers in space and time and then spreads out from that point, taking whatever they've caught--or learned--along the way.  

Where did the group come from?  Where do they go after the event?

To see how a good visualization can answer these questions, check out this [video](https://twitter.com/tectonixgeo/status/1242628347034767361).

# Emulating the Tectonix Approach

I recommend licensing their software.  However, if you already have mobility data and modest Python skills, you can make good progress toward their approach with two simplifying ideas.  

The first simplifying idea is "Meaningful Ticks."  The second is "Dumb JavaScript."

## Meaningful Ticks
The Oxford Dictionary defines a tick as a regular short, sharp sound, especially that made by a clock.  I define a "Meaningful Tick" as a moment that is <em>interesting to the observer</em>.  Meaningful ticks can be regular, e.g. every second, every day, every year, but they needn't be.  What matters is that they are moments in time where the attention of the observer is valuable.  

Note that defining a Meaningful Tick also has the virtue of reducing the amount of data in the visualization.

## Dumb JavaScript
JavaScript is one of the core technologies of the World Wide Web, alongside HTML which describes the structure of a web page and CSS which describes its presentation.

When a web page is loaded, the browser creates a Document Object Model of the page, which is an object oriented representation of an HTML document that acts as an interface between JavaScript and the document itself. This allows the creation of dynamic web pages, because within a page JavaScript can add, change, and remove any of the HTML elements and attributes, change any of the CSS styles, react to all the existing events, and create new events--clearly evidence of intelligent life.

However, I use the phrase "Dumb JavaScript" to emphasize its true role in my emulation of the Tectonix approach.  It quickly and faithfully renders whatever HTML and CSS it has been instructed to render.  All of the intelligence in those instructions--critical to the visual result in the video--is outside the JavaScript and exists before it is invoked.  

Note that Dumb JavaScript also has the virtue of increasing the responsiveness of the visualization.