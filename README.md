# digits-recognition-tfjs

This project is a simple demo shows how to train a tensorflow model with python and deploy it in frontend. The author thanks a great deal to this blog [Recognizing Digits using TensorFlow.js in Google Chrome](https://gogul09.github.io/software/digit-recognizer-tf-js), which make this small project possible. You should check this out if you are interested in tf.js.

Python requirements:
* flask
* flask-cors

This demo has already contained a tensorflowjs model located at server/models/mnist with 98% accuracy on test data set. If you want to re-train the model yourself, you need
* tensorflow
* tensorflowjs

Then run the trainer:
```
python server/train.py
```

You can install all of dependencies mentioned above with pip.

To make this model accessible to a web page, run the server:
```
python server/main.py
```

By default, the server would be running at port 5000. Open http://localhost:5000/, if you see 'Hello World!' in the screen, the server is set up successfully.

Open the file web/index.html in you browser. If everything is ok, there should be something like this:

![demo screenshot](https://i.imgur.com/fRu7WzV.png)

Now you can draw the digit on the black canvas and click the 'recognize' button to see the prediction.
