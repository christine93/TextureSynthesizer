#Texture Synthesizer
A pixel based texture synthesis algorithm, based off of psuedocode from Efros and Leung's 1999 paper. Given an input texture, will used Efros/Leung's patch based algorithm to synthesize a larger texture. For higher quality images, use a higher window size (I recommend at least 7). Images can grow as large as you want. (As long as you're patient enough to wait for it to render ;) )

#USAGE (Octave/matlab) -
This was tested in Octave, however, instructions should be similar if not identical for matlab.
 Load required packages - pkg load image
 Source file        	- source growimage.m
 Call growimage         - e.g. growimage("sampleTextures/fire.JPG",5,20)
 For more information on parameters/individual functions, see function documentation.

Output filename is in format synthesized_<FILENAME>_winsize_<WINSIZE>_<OUTPUTSIZE>x<OUTPUTSIZE>. Currently input image must be in JPG or jpg format. I've included a couple 20x20 output images with varying window sizes an example in the synthesizedTextures directory. 

#Demo
![alt tag](https://raw.github.com/aok5326/TextureSynthesizer/master/sampleTextures/wood.JPG "Input image") ---->	![alt tag](https://github.com/aok5326/TextureSynthesizer/blob/master/synthesizedTextures/synth_wood_winsize_9_20x20.jpg "Output image")


![alt tag](https://raw.github.com/aok5326/TextureSynthesizer/master/sampleTextures/cells.jpg "Input image") ---->	![alt tag](https://github.com/aok5326/TextureSynthesizer/blob/master/synthesizedTextures/synth_cells_winsize_9_20x20.jpg "Output image")



#References:
	http://graphics.cs.cmu.edu/people/efros/research/NPS/alg.html
	http://luthuli.cs.uiuc.edu/~daf/courses/CS-498-DAF-PS/Texture_498.pdf 
	http://eric-yuan.me/texture-synthesis/
	http://www.cs.umd.edu/~djacobs/CMSC426/PS5.doc
	http://www.ics.uci.edu/~dramanan/teaching/cs116_fall08/hw/Project/Texture/
