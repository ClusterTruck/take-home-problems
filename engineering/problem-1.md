# ClusterTruck Take Home Problem

The following is a test designed to ensure you have a fundamental understanding of building data-­driven applications. It is not meant to be challenging, just to qualify your skills and open a conversation.

Please write the code in whatever environment you are comfortable in. Also make the site available publicly through whatever means you might have available and send the URL, login if necessary and either URL or attached code for review.

## Application Requirements

Please write a single page application that utilizes the [New York Times Events API](http://developer.nytimes.com/docs/events_api#) to query for events around NYC and renders them on a [Google Map](https://developers.google.com/maps/documentation/javascript/tutorial).

* Only render the first page of data (paging is not necessary)
* Map should initialize in NYC (40.7127, 74.0059)
* Dragging the map around should fetch events for the new map boundaries
* Events should be rendered on map using Markers
* Event title and details (“web_description” key in payload) should be rendered in an [Info Window](https://developers.google.com/maps/documentation/javascript/examples/infowindow-simple) when the marker is clicked
* Ability to filter out by type of events using the [category Facet Search](http://developer.nytimes.com/docs/events_api#facet-search)
  * Simple toggle checkboxes to filter categories

## Rules

* No frameworks! jQuery, Backbone.JS and Underscore are fine, other than that please write your own code.
* Have fun!

Give it your best shot and get back to me. We're mainly interested in

1. Ability to understand and create such a program.
2. Working code completed in a timely manner. Feel free to be creative with this test. The exact way it looks or behaves is not as important as its functionality and ability to solve the basic problems.

## Notes

Working API key for the New York Times Events API: `1b6ec24de1512db2fae47f5165ce39ea:6:69563513`
