# Installing-Terria-Map
The instruction for installing Terria Map. The easiest way to get started with TerriaJS is to use TerriaMap. TerriaMap is a full-featured application built on TerriaJS, ready to be customized with your own branding and catalog. It is also a great starting point for more in-depth customization.

## Prerequisites
Must Install these soft, if not yet

- The Bash command shell. On macOS or Linux you almost certainly already have this. On Windows, you can easily get it by installing Git for Windows. In the instructions below, we assume you're using a Bash command prompt.

- NodeJS v14 or v16 are supported. You can check your node version by running node --version on the command-line.

- npm v6.0 or later. npm is usually installed automatically alongside the above. You can check your npm version by running npm --version.
yarn v1.19.0 or later. This can be installed using npm install -g yarn@^1.19.0

## Using Git Command

git clone https://github.com/TerriaJS/TerriaMap.git

cd TerriaMap

export NODE_OPTIONS=--max_old_space_size=4096

npm install -g yarn

yarn install && yarn gulp && yarn start

Open at http://localhost:3001


# Language
## adding language: config.json
"languageConfiguration": {
      "enabled": true,
      "debug": false,
      "languages": {
        "en": "English",
        "fr": "Français",
        "km": "Khmer"
      },
      "fallbackLanguage": "en"
## Update langauge 
D:\Projects\webmap\TerriaMap\wwwroot\build\TerriaJS\languages\km
language.json can be downloaded at https://hosted.weblate.org/projects/terriajs/terriajsnext/
![image](https://user-images.githubusercontent.com/118343414/209629897-5a2e1cd9-0b5a-48db-a1a4-634d92de4646.png)


# Change Basemap
edit file wroot/init/simple.json


"baseMaps": {
  "items": [
    {
      "item": {
        "id": "basemap-positron",
        "name": "Base map positron customized name"
      },
      "image": "build/TerriaJS/images/time-series-guide.jpg"
    },
    {
      
        "item": {
          "id": "test-basemap",
          "name": "Voyager with labels",
          "type": "open-street-map",
          "url": "https://basemaps.cartocdn.com/rastertiles/voyager_labels_under/",
          "attribution": "© <a href='https://www.openstreetmap.org/copyright'>OpenStreetMap</a>, © <a href='https://carto.com/about-carto/'>CARTO</a>",
          "subdomains": ["a", "b", "c", "d"],
          "opacity": 1.0
        },
        "image": "build/TerriaJS/images/Australia.png"
      },
    
    {
      "item": {
      "id": "basemap-bing-aerial",
       "name": "Bing Maps Aerial",
      "type": "bing-maps",
      "mapStyle": "Aerial",
      "key":"AnBGbR4bEjAP7vgrY6e0emBLwGYxynzceO4l_7a3ptE_B6SoLJro6PFIE-PXjsOQ",
      "opacity": 1.0
      },
  
  "image": "build/TerriaJS/images/bing-aerial.png",
  "contrastColor": "#ffffff"
  },
  {
    "item": {
    "id": "basemap-bing-aerial-with-labels",
     "name": "Bing Maps Aerial With Labels",
    "type": "bing-maps",
    "mapStyle": "AerialWithLabels",
    "key":"AhvxiItVv2SppHXDx5pVKNUwfYHJwQxTnZeNXv0L7lWaY7E9AQOyPzqAHUM2vPIh",
    "opacity": 1.0
    },
    

"image": "build/TerriaJS/images/bing-aerial.png",
"contrastColor": "#ffffff"
},
{
  "item": {
  "id": "basemap-bing-roads",
   "name": "Bing Maps Aerial With Roads",
  "type": "bing-maps",
  "mapStyle": "Road",
  "key":"xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "opacity": 1.0
  },
  

"image": "build/TerriaJS/images/bing-aerial.png",
"contrastColor": "#ffffff"
}
],

  "enabledBaseMaps": ["basemap-bing-aerial-with-labels","basemap-bing-aerial","basemap-bing-roads","test-basemap","basemap-positron","basemap-black-marble","basemap-natural-earth-II"],
  "defaultBaseMapId": "basemap-positron"
}

## Bing Map Style


    Aerial - Specifies the Aerial map style without road or labels overlay

    AerialWithLabels - Specifies the Aerial map style with road and labels overlay

    Road - Specifies the Roads map style without Aerial overlay


