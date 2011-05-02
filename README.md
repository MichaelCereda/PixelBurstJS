PixelBurstJS is a Canvas libray that allows you to create canvas elements, handle transformations and changes without spending much time on programming.

Copyright (C) 2011 Michael Cereda http://cmyklove.com
  
Build Script
=========  
The build script used is from less.js project https://github.com/cloudhead/less.js  
  
ATTENTION
=========
This project is in the pre-alpha stage, aka it's not working... please check the changes

Usage
=========
Here's an example..  
`

var tar = document.getElementById('target');
 var properties = {
		Stage:{
			width : 640,
			height: 480
		}
	}
 var stage = {
		width: properties.Stage.width,
		height: properties.Stage.height,
		
		Circle:{
			id:'myCircle',
			radius: 100,
			x: properties.Stage.width/2,
			y: properties.Stage.height/2,
			stroke: {
				style : 'cyan',
				width: 20
			},
			endAngle: Math.PI*1.8,
			animate:{ 
				scale:{
					/*  start not defined*/
					end: 2,
					duration: 1000,
					tween: 'sine'
				}
			},
			

		}
	};
	PixelBurst(tar).render(stage);`