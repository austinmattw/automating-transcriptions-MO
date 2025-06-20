# automating-transcriptions-MO
Python code used for automating herbarium specimen transcription in the Missouri Botanical Garden Herbarium.

# Description
This code automates transcription of herbarium specimen images and is designed to process a batch of images in every run of the pipeline. This code is specifically designed for use at the Missouri Botanical Garden Herbarium (MO), but can be modified for use with specimens from other institutions.


The pipeline consists of three steps:

(1) Performing optical character recognition (OCR) on specimen images.

(2) Parsing label text to database fields using the ChatGPT API (from OpenAI).

(3) Formatting the output for upload to Tropicos.org, the Missouri Botancial Garden's database for storing specimen records.


Prior to running the code, the user sets paths to the input folder containing the images, the archive folder where images will be sent after processing, and the output folder where the spreadsheet of specimen data will be saved.

# Requirements
Each session of the pipeline is initialized through the Google Cloud SDK Shell. Running this code requires a Google account and an OpenAI API key.
