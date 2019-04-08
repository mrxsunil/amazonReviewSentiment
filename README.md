# Sentiment Analysis on Amazon Reviews
## Set-up

This runs on Python 3.6.8.

This project requires [fast.ai](https://github.com/fastai/fastai) version 0.7.

* Use the configuration file to set up the environment. I used `conda` to manage the packages and environment. 
* Note that the code below is for cpu, but I have included the environment file for gpu `enviroment.yml`. 

```
conda env create -f environment-cpu.yml
conda activate fastai-cpu
```

Or for updating the environment:

`conda env update -f environment-cpu.yml`


## Download Dataset
* To acquire the dataset for amazon reviews please go Xiang Zhang's Google Drive following this [link]( 
https://drive.google.com/drive/folders/0Bz8a_Dbh9Qhbfll6bVpmNUtUcFdjYmF2SEpmZUZUcVNiMUw1TWN6RDV3a0JHT3kxLVhVR2M)
* Download the file named "amazon_review_full_csv.tar.gz "

## Downloading pre-trained weights

Note that you will have to download the pre-trained language model. I have used the wikitext103 language created by Stephen Merity @ Salesforce research. [Here](http://files.fast.ai/models/wt103/) is a link from fast.ai, and here is a command for the terminal:

`$ wget -nH -r -np -P {PATH} http://files.fast.ai/models/wt103/`

