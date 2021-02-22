# Build your own facial recognition system: To work even with a face mask!
![](https://cdn-images-1.medium.com/max/1250/1*HVWXwbp_i1G7_I5YDKALnA.png =20)

### Introduction
Recently, a neighbor from my building confused me with my sister for the 5th time. She says that I and my sister look very much alike for her to the point of confusing us. A week ago I finally submitted a project for an AI subject I'm taking while doing Erasmus in Budapest.
In this project, now article, I create a facial recognition system from scratch with a Convolutional Neural Network(CNN) structure using Keras, to recognize me and my sister.

Later on, in this project and Notebook, I build another model using the Transfer Learning technique, to reach higher validation accuracy scores and when testing with new and different photos, as well as when using the web camera with different lighting.
In this tutorial I create two models: One from scratch and another one with a pre-trained model
All along, for both of the models, applying Data Augmentation as well. With this technique, I was able to augment data up to 2794 photos, by randomly adding or removing brightness, saturation, and more angles of the faces by flipping them and rotating them. It's because of this Data Augmentation that I could create a more robust model.

From the augmented resulting images, 1871 were used to training the model and 923 for the test validation set.

![The first model (Build from scratch) recognizing me in recent photo.](https://cdn-images-1.medium.com/max/938/1*GeEHUmsVwNEB95aK09RgOw.png)

The first model (Build from scratch) recognizing me in recent photo.The model is tested in different types of photos taken from different cameras/phones, different times, and different looks/make-up. With a confusion matrix, it's possible to see how the models can have more precision when predicting one of the classes (in this case either for my sister's face or mine).
The models are saved as ".h5" files for easy portability, as well as the complete dataset of images created are compressed as ".npz" files for the same reason.

At the end of this project, I was able to make the model recognize me even when using a face mask. Very interesting for me.

![Photo of me after winning in my first Escape Room](https://cdn-images-1.medium.com/max/1250/1*BvO6uQfdn6cUqxueWuWRPQ.png)
[](https://cdn-images-1.medium.com/max/1250/1*Uc5jGDIqs0PZDOrxfI9odw.png)
