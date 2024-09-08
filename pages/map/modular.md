---
title: map
date: '09:27 08-09-2024'
content:
    items: '@self.modular'
hide_page_title: false
show_sidebar: true
hide_git_sync_repo_link: false
sitemap:
    lastmod: '08-09-2024 09:27'
---

# NEBA
[map-leaflet lat=51.505 lng=-0.09 zoom=10 mapname=neighbourhood variant=neighbourhood scale ]
[a-markers markerColor="darkblue"
iconColor="white"
]
[{ "lat": 37.7749, "lng": -122.4194, "icon": "home", "title": "Home Position" } ]
[/a-markers]
[a-markers icon=""]
[  { "lat": 51.505,  "lng": -0.09 , "text": 1, "draggable": true  },
{ "lat":  51.515,  "lng": -0.1 , "text": 2, "markerColor": "cadetblue" },
{ "lat":   51.515,  "lng": -0.14, "text": 3, "spin": true },
{ "lat":   51.505,  "lng": 0, "text": 4, "spin": false },
{ "lat":   51.525,  "lng": -0.01, "icon": "coffee", "markerColor": "red", "title": "Lovely bistro"}
]
[/a-markers]
[/map-leaflet]

# San Fransisco Transport
[map-leaflet lat=37.7749 lng=-122.4194 zoom=13 mapname=transd variant=transport-dark ]
[a-markers markerColor="lightblue"
iconColor="white"
]
[{ "lat": 37.7749, "lng": -122.4194, "icon": "home", "title": "Home Position" } ]
[/a-markers]
[a-markers icon=""]
[  { "lat": 37.775,  "lng": -122.48 , "text": 1, "draggable": true  },
{ "lat":  37.77,  "lng": -122.414 , "text": 2, "markerColor": "pink" },
{ "lat":   37.765,  "lng": -122.409, "text": 3, "spin": true },
{ "lat":   37.76,  "lng": -122.3995, "text": 4, "spin": false },
{ "lat":   37.755,  "lng": -122.499, "icon": "coffee", "markerColor": "lightred", "title": "Lovely bistro"}
]
[/a-markers]
[/map-leaflet]