# Final Project - One Film, Four Flavors

Yudi Wang, yuw043@ucsd.edu


## Abstract Proposal

I do love the the famous bamboo fighting scene from the film *Crouching Tiger, Hidden Dragon* and feel it can be understood from different angles. In this project, I combined the video-style-transfer and the audio-style-transfer. I trim 4 clips from the original movie and try to tranfer it into 4 different style: playful, sad, angry and horrible. In order to do this, I adopt different stylized video and stylized audio created by the algorithm.

Basic idea of video style transfer is first dividng the video into a sequence of frames, then apply the arbitrary style transfer algorithm on these frames one by one. The last simple step is combining these stylized frames together and thus we have a style transferred ballet dance video. For the style transfer step, I choose the arbitray-style-transfer model which is flexible and manageable. The original video format is mp4 and the reansferred one is avi which has small memory assumption.

Basic idea of audio style transfer


## Project Report

Upload your project report (4 pages) as a pdf with your repository, following this template: [google docs](https://drive.google.com/open?id=1mgIxwX1VseLyeM9uPSv5GJQgRWNFqtBZ0GKE9d4Qxww).

## Model/Data

- For the video style transfer part:

The adopted model is arbitrary style transfer algorithm which is based on pretrained VGG-19. For the style picture, I collected via google and after try all of them, only reserve the good ones. The final picked style picture are shown as below:

Video document is scrapped from Youtube


- For the audio style transfer part, code is adopted from the colab seedbank.

## Code

Following code is run on colab platform:

- trained models - Video_Style_Transfer.ipynb & Audio_Style_Transfer.ipynb


## Results

In order to get the best result, I tried different chinese ink painting style images, which is shown as below:

## Technical Notes

For the style transfer part, I use the code from the below repository: https://github.com/elleryqueenhomels/arbitrary_style_transfer

Required package: cv2 and lower version of scipy(1.1.0).

Code is worked on colab platform which is easy to install the older version of scipy(1.1.0).

## Reference

Arbitrary_Style_Transfer https://github.com/elleryqueenhomels/arbitrary_style_transfer
