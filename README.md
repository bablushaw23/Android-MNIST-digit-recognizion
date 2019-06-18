Main thing was actually built using Javascript and then the webpage(No internet required) is then fit inside app.

To build this app within reasonable size and resources i took android's browser support. For this i made a webpage where small and tuned version of neural network's code is written in javascript. No dependencies, just simple maths.

You'll find the webpage inside assets folder under apps->src->main.
Technical explaination is written in webpage itself.

Below is most abstract form of logic about how the code works:

If you have basic knowledge of machine learning or most precisely, Neural network then:

We know that to predict something the net needs set of theta(s)( or weights, bias in some tounge ). These found by model. It was easy for me to find
the model which could give me 97% accuracy, from google. All i need to collect the mnist database and run the model. After successfullt testing the model for accuracy i collected the thetas into thetas.js file from there. 

That model was build of 300(301 with bias) node at 1st layer and 10 node for 2nd one.

Only thing remain is to collect user input in the form as same as while training the net. For this i used a 280*280 Js canvas and later reduced to
 28*28 n size.

after getting the png image from canvas, I extracted the image data and fed to the net along with theta(s) leaving remain onto the smartphone's processor speed to do a matrix calculation.

Sigmoid is used as activation function.

That's all. 
If you get anything ambigious, you are free to contact me.
