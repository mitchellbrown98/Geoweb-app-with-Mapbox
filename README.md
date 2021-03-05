application.py:
There is only 1 route needed for this lab

1. @app.route("/") 
	- This route passes the username, style_id, and access token for the Mapbox tile layer, and renders the index.html page.
	

Index.html:
- This page contains the original stadia map tile layer from lab 2, which is initially seen when you load the page. 
- You have the ability to toggle between the original lab 2 map, or the new lab 3 map, which was created in mapbox studio, and has the new traffic incident dataset on it. You can also enter full screen mode. 
- For this lab, the focus is on the traffic points and roadways they occur on, so the map background has been darkened, along with the green features, water ports, airports, pedestrian roadways, etc as they are not as relevant. The labels have been updated as well for ease of viewing with the dark background.
- Orange greatly contrasts with green, so I have made the traffic points orange, on top of the various green roadways to ensure they easily stand out.
- I chose a radius of 4px for the traffic points, as that size will fit inside the roadway when you are zoomed into the map. The points will also adjust their size based on the zoom layer, so it is easy to see where they are grouped together when you zoom out, but can be easily identified and differentiated when you zoom in. I chose to use no blur, and full opacity so the points appear sharp and easily stand out.
- I chose to include the natural features, place labels, point of interest labels, road networks, terrain, transit, and walking & cycling components as these can aid in the visualization and correlation of the traffic incident dataset. 
