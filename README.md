unity3d-texturepackerimporter [![Build Status](https://travis-ci.org/haysclark/unity3d-texturepackerimporter.png)](https://travis-ci.org/haysclark/unity3d-texturepackerimporter)
=============================

Unity3D - Texture Packer Importer
http://www.texturepacker.com/

## Authors
* Mitch Thompson
* Harald Lurger
* Hays Clark

## Video Tutorial
There is a tutorial for this plugin here:
http://www.youtube.com/watch?v=CHQmvC1pqaY

## Instructions
How to import texture sheets from Texture Packer

## TexturePacker settings:
	Data Format:  Unity3D (or JSON Hashtable, then change extension from .json to .txt so Unity picks it up as a text asset)
	Allow rotation is OK
	Everything else at your discretion
	Power of 2 output textures are suggested.
	
## Unity process:
	Create a folder in your Assets/ directory for your imported sprites.
	Copy the TXT and Image file (PNG, TGA, etc) into that folder.
	Your paths should look something like:
		Assets/MySprite/MySprite.txt
		Assets/MySprite/MySprite.png
			
## Shaders:
	Transparent Unlit - 
		The default shader for all imported sprite sheets.
	Opaque Unlit - 
		nontransparent tintable shader great for drawing backgrounds that don't need alpha.  Very efficient.
	Vertex Color - 
		Does not have an inspector-tweakable color property.  All colors must be set by altering the colors[] or colors32[] array of a given mesh.  
		Supports both texture alpha and vertex color alpha.
