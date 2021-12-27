# Image Captioning

Keras.io example

Flickr8K dataset comprises over 8000 images, that are each paired with five different captions

Our image captioning architecture consists of three models:
1. A CNN: used to extract the image features
2. A TransformerEncoder: The extracted image features are then passed to a Transformer - based encoder that generates a new representation of the inputs
3. A TransformerDecoder: This model takes the encoder output and the text data (sequences) as inputs and tries to learn to generate the caption.