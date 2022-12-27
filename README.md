# Installing-Terria-Map
The instruction for installing Terria Map. The easiest way to get started with TerriaJS is to use TerriaMap. TerriaMap is a full-featured application built on TerriaJS, ready to be customized with your own branding and catalog. It is also a great starting point for more in-depth customization.

##Prerequisites
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
##adding language: config.json
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
language.json can be downloaded athttps://hosted.weblate.org/projects/terriajs/terriajsnext/
![image](https://user-images.githubusercontent.com/118343414/209629897-5a2e1cd9-0b5a-48db-a1a4-634d92de4646.png)


 
