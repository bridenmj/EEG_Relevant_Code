# EEG_Relevant_Code
contains relevant code for creating images, separating images, and classifying. eeg_full.zip is on google drive.

## 1: Construct images
### a: 
  download eeg_full.zip from google drive and scp to server, unzip.
### b: 
  use gz_to_csc.<ext> to unzip all .gz files with eeg_full and convert to .csv files

### c:
  construct_images_from_multinnel_eeg.<ext> to convert each .csv file to img. you will need to set path_to_imgs to the following
  ~/eeg_full/S1/control
  ~/eeg_full/S1/alcoholic
  ~/eeg_full/S2/control
  ~/eeg_full/S2/alcoholic
  ~/eeg_full/S3/control
  ~/eeg_full/S3/alcoholic
  
### d:
 Use organize_img.<ext> on S1,S2,S3, or all .csv files pooled to splite photos into training, validation, and training sets.
 
### e:
 use inception_V3_model_code.<ext> to train.
  
