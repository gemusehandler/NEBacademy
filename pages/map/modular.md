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

[map-leaflet lat=51.505 lng=-0.09 zoom=13 mapname=neighbourhood style=neighbourhood]
[a-markers markerColor="darkblue"
iconColor="white"]
[{ "lat": 37.7749, "lng": -122.4194, "icon": "home", "title": "Home Position" } ]
[/a-markers]
[a-markers icon=""]
[  {"icon": "coffee", "title": "popup text", "lat": 51.505,  "lng": -0.09 , "text": 1, "draggable": true  },
{ "lat":  51.515,  "lng": -0.1 , "text": 2, "markerColor": "cadetblue" },
{ "lat":   51.515,  "lng": -0.14, "text": 3, "spin": true },
{ "lat":   51.505,  "lng": 0, "text": 4, "spin": false },
{ "lat":   51.525,  "lng": -0.01, "icon": "coffee", "markerColor": "red", "title": "Lovely bistro"}]
[/a-markers]
[/map-leaflet]

{assets:css order:5}
/user/plugins/map-marker-leaflet/assets/leaflet.extra-markers.min.css
{/assets}

{assets:js order:10}
/user/plugins/map-marker-leaflet/assets/leaflet.extra-markers.min.js
{/assets}

{assets:inline_js}
jQuery(document).ready(function () {
    var map = L.map('neighbourhood').setView([51.505, -0.09],13);
    L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: 'Map data &copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors',
        maxZoom: 17
                    }).addTo(map);
    
     L.marker([37.7749,-122.4194], {
        icon: L.AwesomeMarkers.icon({
          markerColor: 'darkblue',
          iconColor: 'white'
                    , icon: 'home'                    })
          , title: "HomePosition"                  }).addTo(map);

    L.marker([51.505,-0.09], {
        icon: L.AwesomeMarkers.icon({
          markerColor: 'blue',
          iconColor: 'white'
                    , icon: '1'          , text: "1"          })
                    , draggable: 1        }).addTo(map);
    L.marker([51.515,-0.1], {
        icon: L.AwesomeMarkers.icon({
          markerColor: 'cadetblue',
          iconColor: 'white'
                    , icon: '1'          , text: "2"          })
                            }).addTo(map);
    L.marker([51.515,-0.14], {
        icon: L.AwesomeMarkers.icon({
          markerColor: 'blue',
          iconColor: 'white'
          , spin: '1'          , icon: '1'          , text: "3"          })
                            }).addTo(map);
    L.marker([51.505,0], {
        icon: L.AwesomeMarkers.icon({
          markerColor: 'blue',
          iconColor: 'white'
                    , icon: '1'          , text: "4"          })
                            }).addTo(map);
    L.marker([51.525,-0.01], {
        icon: L.AwesomeMarkers.icon({
          markerColor: 'red',
          iconColor: 'white'
                    , icon: 'coffee'                    })
          , title: "Lovelybistro"                  }).addTo(map);


});
{/assets}