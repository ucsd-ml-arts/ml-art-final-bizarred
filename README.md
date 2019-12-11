# Final Project - One Film, Four Flavors

Yudi Wang, yuw043@ucsd.edu

<img src="https://github.com/ucsd-ml-arts/ml-art-final-bizarred/blob/master/frame0436.jpg" width="500">

## Abstract Proposal

I do love the the famous bamboo fighting scene from the film *Crouching Tiger, Hidden Dragon* and feel it can be understood from different angles. In this project, I combined the video-style-transfer and the audio-style-transfer. I trim 4 clips from the original movie and try to tranfer it into 4 different style: playful, sad, angry and horrible. In order to do this, I adopt different stylized video and stylized audio created by the algorithm.

Basic idea of video style transfer is first dividng the video into a sequence of frames, then apply the arbitrary style transfer algorithm on these frames one by one. The last simple step is combining these stylized frames together and thus we have a style transferred ballet dance video. For the style transfer step, I choose the arbitray-style-transfer model which is flexible and manageable. The original video format is mp4 and the reansferred one is avi which has small memory assumption.

Basic idea of audio style transfer is synthesizes audio "content" and "style" independently using the magnitudes of a short time Fourier transform, shallow convolutional networks with randomly initialized filters, and iterative phase reconstruction with Griffin-Lim. In order to make comparsion between different style, I adopt same music content with different style. The result is quite interesting.


## Project Report

Upload your project report (4 pages) as a pdf with your repository, following this template: [google docs](https://drive.google.com/open?id=1mgIxwX1VseLyeM9uPSv5GJQgRWNFqtBZ0GKE9d4Qxww).

## Model/Data

- For the video style transfer part: Video_Style_Transfer-2.ipynb

The adopted model is arbitrary style transfer algorithm which is based on pretrained VGG-19. For the style picture, I collected via google and after try all of them, only reserve the good ones. The final picked style picture are shown as below:

<img src="https://github.com/ucsd-ml-arts/ml-art-final-bizarred/blob/master/Video%20Stylized%20Result/Style%20Images.png" width="800">
Video document is scrapped from Youtube

1. https://www.youtube.com/watch?v=FEPf1M0n5SM&t=139s

2. https://www.youtube.com/watch?v=KXIJv1NoXmo
（Crouching Tiger, Hidden Dragon (7/8) Movie CLIP - Bamboo Forest Fight (2000) HD）

- For the audio style transfer part, code is adopted from the colab seedbank: Audio_Style_Transfer.ipynb

  1. Content Music: 
  
  https://www.youtube.com/watch?v=S5AjtMNnWf0&list=PLW2r9GbkzeG3H2IjCanmZnlJGwg8Ui0no&index=1
  
  
  （Crouching Tiger, Hidden Dragon OST #1 - Crouching Tiger, Hidden Dragon）
  
  2. Style Music: 
  


  > Part 1: https://www.youtube.com/watch?v=ZvJE_BEADpI （食之契約 櫻之島BGM：如夢似幻）
  
  > Part 2: https://www.youtube.com/watch?v=m1eKVWn0vls (Dans la Maison Theme Soundtrack - Philippe Rombi (HD 1080P))
  
  > Part 3：https://www.youtube.com/watch?v=JOb0AuZ9Gzs (Mark Petrie - Go Time Extended)
  
  > Part 4: https://www.youtube.com/watch?v=3G2TF4jgJCs&list=PLzBLIrZhm6tZYLPWUh_rRmjq_6DH-0PpO&index=3 (Requiem for a Dream [Música de Suspense] Full theme song)


## Code

Following code is run on colab platform:

- trained models - Video_Style_Transfer.ipynb & Audio_Style_Transfer.ipynb


## Results

> For audio style transfer:

<img src="https://github.com/ucsd-ml-arts/ml-art-final-bizarred/blob/master/Audio%20Stylized%20Result/Audio%20Result.png" width="800">

Process can be found in the following link:

https://drive.google.com/file/d/19J2Poh7G0ao1kJXAwahaEhx9if50gdFH/view?usp=sharing


> For video style transfer:

In order to get the best result, I tried tens of painting style images. Final result are shown as below:
<img src="https://github.com/ucsd-ml-arts/ml-art-final-bizarred/blob/master/Video%20Stylized%20Result/style.001.jpeg" width="500">
<img src="https://github.com/ucsd-ml-arts/ml-art-final-bizarred/blob/master/Video%20Stylized%20Result/style.002.jpeg" width="500">
<img src="https://github.com/ucsd-ml-arts/ml-art-final-bizarred/blob/master/Video%20Stylized%20Result/style.003.jpeg" width="500">
<img src="https://github.com/ucsd-ml-arts/ml-art-final-bizarred/blob/master/Video%20Stylized%20Result/style.004.jpeg" width="500">

The final version of the video can be viewed at the below link:

https://drive.google.com/file/d/12pjGmoAiRq0AkjolQnozrbZgFUJSfF16/view?usp=sharing


## Technical Notes

- For the video style transfer part, I use the code from the below repository: https://github.com/elleryqueenhomels/arbitrary_style_transfer

- Required package: cv2 and lower version of scipy(1.1.0).

- For the audio style transfer part, I use the code offered by colab seedbank:
https://colab.research.google.com/drive/18_DckMGM-fsSthIqZI9sOAlY6I3plDLD?sandboxMode=true#forceEdit=true&offline=true&sandboxMode=true

- Code is worked on colab platform which is easy to install the older version of scipy(1.1.0).


## Reference

- Arbitrary_Style_Transfer https://github.com/elleryqueenhomels/arbitrary_style_transfer

- Audio Style Transfer https://colab.research.google.com/drive/18_DckMGM-fsSthIqZI9sOAlY6I3plDLD?sandboxMode=true#forceEdit=true&offline=true&sandboxMode=true

> [1]. D. Ulyanov and V. Lebedev, “Audio texture synthesis and style transfer,” 2016

> [2]. P. K. Mital. _Time Domain Neural Audio Style Transfer_. Presented at the Workshop on Machine Learning for Creativity and Design at the Neural Information Processing Systems Conference 2017 (NIPS2017), December 3 – 9, 2017.  [arxiv](https://arxiv.org/abs/1711.11160) [workshop](https://nips2017creativity.github.io)


