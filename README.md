# image_recognizer_sketch1

Image recognizer sketch 1 (still needs refinement to adapt to my scenario).  This idea comes almost exclusively from code from **Adrian Rosebok**-- his code is useful though its intent was to run on small computers and small datasets. His intent was to put the identifier/classifier on an iPhone, whereas I am targeting a research problem best addressed on an HPC (highly parallel job partioning) and training testing set based on millions of images!

I borrowed the Google image dowloader code from Hardik Vassas excellent project (https://github.com/hardikvasa/google-images-download).  This downloader allows us to "bootstrap" our dataset for model training and program testing.  This project ultimately will not use this since we have very extensive human-identified dataset to train our model.

major credit to Adrian Rosebok (totally recommend reading his books)

I adapted this idea from:

  1. Deep Learning for Computer Vision, Adrian Rosebock (2018)
  2. Keras and Convolutional Neural Networks (pyimagesearch.com)
  3. Practical Python and Open CV 4rth edition, Adrian Rosebock

Google Image downloader was written by Hardik Vassa

https://github.com/hardikvasa/google-images-download


My project sketch part 2 and 3 will take the ideas from sketch 1 and refine the model to work against more detailed imagery collected from camera traps in the serengeti national wildlife preserve

 ## part 2
- classifier will work against a directory and provide CSV output rather than visual inspection

## part 3
- will use a 2-stage classifier.  Stage 1 will identify "interesting" images.  Stage 2 will provide classification on a species trained model.
