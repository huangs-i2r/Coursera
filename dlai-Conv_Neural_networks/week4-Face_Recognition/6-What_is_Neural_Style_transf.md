
One of the most fun and exciting applications of ConvNet recently has been Neural Style Transfer. You get to implement this yourself and generate your own artwork in the problem exercise. But what is Neural Style Transfer? Let me show you a few examples. Let's say you take this image, this is actually taken from the Stanford University not far from my Stanford office and you want this picture recreated in the style of this image on the right. This is actually Van Gogh's, Starry Night painting. What Neural Style Transfer allows you to do is generated new image like the one below which is a picture of the Stanford University Campus that painted but drawn in the style of the image on the right. In order to describe how you can implement this yourself, I'm going to use C to denote the content image, S to denote the style image, and G to denote the image you will generate. Here's another example, let's say you have this content image so let's see this is of the Golden Gate Bridge in San Francisco and you have this style image, this is actually Pablo Picasso image. You can then combine these to generate this image G which is the Golden Gate painted in the style of that Picasso shown on the right. The examples shown on this slide were generated by Justin Johnson. What you'll learn in the next few videos is how you can generate these images yourself. In order to implement Neural Style Transfer, you need to look at the features extracted by ConvNet at various layers, the shallow and the deeper layers of a ConvNet. Before diving into how you can implement a Neural Style Transfer, what I want to do in the next video is try to give you better intuition about whether all these layers of a ConvNet really computing. Let's take a look at that in the next video.