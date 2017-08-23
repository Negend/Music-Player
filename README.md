# Music Player
A simple music player made from scratch
## Features
 * play and pause
 * skip to next or previous track
 * progress bar
 * option to select from playlist
 * display cover photo
## Tools
	* Jquery and html5 audio element
	* bootstrap for icons
## Installation

In command line run this script to run

````
git clone git@github.com:Negend/Music-Player.git
````
 Copy the following script into head tag for in html page

 ````
 <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.js"></script>
	<script type="text/javascript" src='player-main.js'></script>
	<link rel="stylesheet" type="text/css" href="player-style.css">
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css">
````
"music-cover" class can be found in the index.html wherever this class appears in the document the cover photo will appear as its background image


there is no function to read the songs folder into the music player. they must be hard coded to link to each other 
by adding or replacing appropriately in this format found in file:player-main.js


````
var tracks = [
	{
		song : 'song/yo.mp3',
		cover : 'song/yo.webp',
		title : 'Welcome'
	},
	
	{
		song:'song/drunk.mpeg',
		cover : 'song/drunk.jpg',
		title:'Drunk Loving'
	},
	
	{	
		song:'song/gas.mp3',
		cover : 'song/gas.jpg',
		title:'Gassed'
	},

	{	
		song:'song/prowl.mpeg',
		cover : 'song/prowl.jpg',
		title:"Prowl O' Lion"
	}
]
````
The player is wrapped in a div box with id 'music-player-box' the css at the moment is this and can be manipulated to fit in website
````
#music-player-box{
	width: 500px;
	text-align: center;
	display: inline-block;
}
````
 

## Developement
A method to read the songs folder and create the playlist without hardcoding will be part of the next tasks
