# Sneaker Classifier CNN

See the CNN in action: [sneakername](https://sneakername.com)

A convolutional neural network that classifies up to 900 sneakers with 90% accuracy. Trained using the [fast.ai](https://www.fast.ai) libary. 

## How this was build

First I scraped the [StockX](https://stockx.com) website to get a large csv file of product data. I modifed an existing script from [zpencerguy](https://github.com/zpencerguy/fmarket) to create a new script that worked on the StockX website. See here: [StockX-scraper](https://github.com/SebastiaanJohn/stockx-scraper). 

Next, I cleaned the data and put all the product names in a text file, and used a script to download 100 images per sneaker from google. This got me 90k images total. Then I cleaned the data manually which left me with 52k usable images.

Finally, I used the Fastai libary to train a convolutional neural network on the images and got an decent accuracy of 90%.

It's far from perfect, but it was a fun experiment.
