
You have learned a lot about ConvNets, everything ranging from the architecture of the ConvNet to how to use it for image recognition, to object detection, to face recognition and neural-style transfer. And even though most of the discussion has focused on images, on sort of 2D data, because images are so pervasive. It turns out that many of the ideas you've learned about also apply, not just to 2D images but also to 1D data as well as to 3D data. Let's take a look. In the first week of this course, you learned about the 2D convolution, where you might input a 14 x 14 image and convolve that with a 5 x 5 filter. And you saw how 14 x 14 convolved with 5 x 5, this gives you a 10 x 10 output. And if you have multiple channels, maybe those 14 x 14 x 3, then it would be 5 x 5 that matches the same 3. And then if you have multiple filters, say 16 filters, you end up with 10 x 10 x 16. It turns out that a similar idea can be applied to 1D data as well. For example, on the left is an EKG signal, also called an electrocardioagram. Basically if you place an electrode over your chest, this measures the little voltages that vary across your chest as your heart beats. Because the little electric waves generated by your heart's beating can be measured with a pair of electrodes. And so this is an EKG of someone's heart beating. And so each of these peaks corresponds to one heartbeat. So if you want to use EKG signals to make medical diagnoses, for example, then you would have 1D data because what EKG data is, is it's a time series showing the voltage at each instant in time. So rather than a 14 x 14 dimensional input, maybe you just have a 14 dimensional input. And in that case, you might want to convolve this with a 1 dimensional filter. So rather than the 5 by 5, you just have 5 dimensional filter. So with 2D data what a convolution will allow you to do was to take the same 5 x 5 feature detector and apply it across at different positions throughout the image. And that's how you wound up with your 10 x 10 output. What a 1D filter allows you to do is take your 5 dimensional filter and similarly apply that in lots of different positions throughout this 1D signal. And so if you apply this convolution, what you find is that a 14 dimensional thing convolved with this 5 dimensional thing, this would give you a 10 dimensional output. And again, if you have multiple channels, you might have in this case you can use just 1 channel, if you have 1 lead or 1 electrode for EKG, so times 5 x 1. And if you have 16 filters, maybe end up with 10 x 16 over there, and this could be one layer of your ConvNet. And then for the next layer of your ConvNet, if you input a 10 x 16 dimensional input and you might convolve that with a 5 dimensional filter again. Then these have 16 channels, so that has a match. And we have 32 filters, then the output of another layer would be 6 x 32, if you have 32 filters, right? And the analogy to the the 2D data, this is similar to all of the 10 x 10 x 16 data and convolve it with a 5 x 5 x 16, and that has to match. That will give you a 6 by 6 dimensional output, and you have 32 filters, that's where the 32 comes from. So all of these ideas apply also to 1D data, where you can have the same feature detector, such as this, apply to a variety of positions. For example, to detect the different heartbeats in an EKG signal. But to use the same set of features to detect the heartbeats even at different positions along these time series, and so ConvNet can be used even on 1D data. For along with 1D data applications, you actually use a recurrent neural network, which you learn about in the next course. But some people can also try using ConvNets in these problems. And in the next course on sequence models, which we will talk about recurring neural networks and LCM and other models like that. We'll talk about the pros and cons of using 1D ConvNets versus some of those other models that are explicitly designed to sequenced data. So that's the generalization from 2D to 1D. How about 3D data? Well, what is three dimensional data? It is that, instead of having a 1D list of numbers or a 2D matrix of numbers, you now have a 3D block, a three dimensional input volume of numbers. So here's the example of that which is if you take a CT scan, this is a type of X-ray scan that gives a three dimensional model of your body. But what a CT scan does is it takes different slices through your body. So as you scan through a CT scan which I'm doing here, you can look at different slices of the human torso to see how they look and so this data is fundamentally three dimensional. And one way to think of this data is if your data now has some height, some width, and then also some depth. Where this is the different slices through this volume, are the different slices through the torso. So if you want to apply a ConvNet to detect features in this three dimensional CAT scan or CT scan, then you can generalize the ideas from the first slide to three dimensional convolutions as well. So if you have a 3D volume, and for the sake of simplicity let's say is 14 x 14 x 14 and so this is the height, width, and depth of the input CT scan. And again, just like images they'll all have to be square, a 3D volume doesn't have to be a perfect cube as well. So the height and width of a image can be different, and in the same way the height and width and the depth of a CT scan can be different. But I'm just using 14 x 14 x 14 here to simplify the discussion. And if you convolve this with a now a 5 x 5 x 5 filter, so you're filters now are also three dimensional then this would give you a 10 x 10 x 10 volume. And technically, you could also have by 1, if this is the number of channels. So this is just a 3D volume, but your data can also have different numbers of channels, then this would be times 1 as well. Because the number of channels here and the number of channels here has to match. And then if you have 16 filters did a 5 x 5 x 5 x 1 then the next output will be a 10 x 10 x 10 x 16. So this could be one layer of your ConvNet over 3D data, and if the next layer of the ConvNet convolves this again with a 5 x 5 x 5 x 16 dimensional filter. So this number of channels has to match data as usual, and if you have 32 filters then similar to what you saw was ConvNet of the images. Now you'll end up with a 6 x 6 x 6 volume across 32 channels. So 3D data can also be learned on, sort of directly using a three dimensional ConvNet. And what these filters do is really detect features across your 3D data,
8:08
CAT scans, medical scans as one example of 3D volumes. But another example of data, you could treat as a 3D volume would be movie data, where the different slices could be different slices in time through a movie. And you could use this to detect motion or people taking actions in movies. So that's it on generalization of ConvNets from 2D data to also 1D as well as 3D data. Image data is so pervasive that the vast majority of ConvNets are on 2D data, on image data, but I hope that these other models will be helpful to you as well. So this is it, this is the last video of this week and the last video of this course on ConvNets. You've learned a lot about ConvNets and I hope you find many of these ideas useful for your future work. So congratulations on finishing these videos. I hope you enjoyed this week's exercise and I look forward also to seeing you in the next course on sequence models.