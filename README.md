# Vehicle-Price-Prediction_through_ANPR
LPR sometimes called ALPR (Automatic License Plate Recognition) has 3 major stages.

License Plate Detection:

This is the first and probably the most important stage of the system. It is at this stage that the position of the license plate is determined. The input at this stage is an image of the vehicle and the output is the license plate. In this stage, the position of the rectangular number plate in the input image is detected. Then the detected number plate is extracted out from the image, to serve as the input to the next stage i.e., Character Segmentation stage. The approach used in this work for License Plate detection is based on Otsu BInarization and Connected Component Analysis (CCA).

Character Segmentation:

It’s at this stage the characters on the license plate are mapped out and segmented into individual images. Character segmentation is the procedure of extracting the characters and numbers from the license plate image. Diverse aspects make the character segmentation task complicated, like image noise, plate frame, space mark, plate’s rotation and light variance. A number of procedures have been proposed for character segmentation to overcome these problems. After removing the plate borders in the previous step, this step starts with removing the noise from the plate. The approach used in this work for character segmentation is based on Adaptive thresholding, morphological processing and contour tracing.

Character Recognition:

This is where we wrap things up. The characters earlier segmented are identified here. We’ll be using machine learning for this. After the segmentation of elements (characters and numbers), the final module in the license plate recognition process is character recognition. It’s at this stage we introduce the concept of machine learning. Although there are many techniques present and applied for character recognition like statistical, syntactic and neural networks in this research, character recognition is performed by using feature extraction. We’ll be taking the path of supervised learning because we already have an idea of how As, Bs and all the letters look like. Supervised learning can be divided into two categories; classification and regression. Character recognition belongs to the classification category.

To execute this phase, we need to get a training data set, choose a supervised learning classifier, train a model, test the model and see how accurate it is, then use the model for prediction.

There are several classifiers we can use with each of them having its advantages and disadvantages. We’ll use SVC (support vector classifiers) for this task. I chose to use SVC because it gave me the best performance. However, this does not necessarily mean that SVC is the best classifier.
