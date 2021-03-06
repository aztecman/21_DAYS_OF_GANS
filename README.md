# 21_DAYS_OF_GANS
This repo is a journal of my progress experimenting with Generative Adversarial Networks in Python over a series of 21 days.
## Day 1: 
**Today's Progress:**
##### Reading: Explored the first 9 articles of [Jonathan Hui's GAN series on Medium](https://medium.com/@jonathan_hui/gan-gan-series-2d279f906e7b)
##### Coding: modified the code to use cifar100 instead of MNIST

**Link to code:** [here](https://colab.research.google.com/drive/1v1cb2iYof5KSdbm6-j381csR1OCWtZaq)

**Results / Thoughts:**

![cifar100 results](https://raw.githubusercontent.com/aztecman/21_DAYS_OF_GANS/master/cifar100_400EPOCHS.png)
![cifar100 color-results](https://raw.githubusercontent.com/aztecman/21_DAYS_OF_GANS/master/day1_cifar100_400EPOCHS_color.png)

##### My results are rather blurry, but I get the sense that they would improve with further training. Just before going to bed I discovered how to make them color! Well I guess sleep can wait another hour...

**Future Work:**
- Read the rest of Jonathan Hui's articles on Medium
- Read [NIPS 2016 Tutorial: Generative Adversarial Networks](https://arxiv.org/abs/1701.00160)
- Reread [Open Questions About Generative Adversarial Networks](https://distill.pub/2019/gan-open-problems/)
- Code a simple GAN in pure Numpy
- Try generating flowers
- Explore CGANs and infoGANs
- Try out the GAN exercises from [Chapter 3 of Hands on Deep Learning for Games](https://github.com/PacktPublishing/Hands-On-Deep-Learning-for-Games/tree/master/Chapter03/Chapter_3)

**Resources:**
#### [GAN Tutorial - Tensorflow 2.0 Alpha](https://colab.research.google.com/github/tensorflow/docs/blob/master/site/en/r2/tutorials/generative/dcgan.ipynb)

## Day 2: 
**Today's Progress:**
##### Reading: read the remaining articles from [Jonathan Hui's GAN series on Medium](https://medium.com/@jonathan_hui/gan-gan-series-2d279f906e7b)
##### Coding: 
- modified WGAN code to display the images correctly, rather than bleached out
- tried 800 epochs (2X yesterday) for the DCGAN

**Link to code:** [here](https://colab.research.google.com/drive/1fMJKhZy788SMWKCdqemCNCXEC6qaVJ_u)

**Results / Thoughts:**

![cifar100 wgan results](https://raw.githubusercontent.com/aztecman/21_DAYS_OF_GANS/master/day2_wgan_cifar100_4000EPOCHS.png)
![cifar100 wgan results improved](https://raw.githubusercontent.com/aztecman/21_DAYS_OF_GANS/master/day2_wgan_cifar100_4000EPOCHS_color_adjusted.png)

##### Today's results are basically crap. On the plus side there is always tomorrow

**Future Work:**
- Explore CGANs and ACGANs
- Generate some outer-space textures
- Generate Insects
- Generate Koi
- Generate Faces
- Generate UV maps for 3d objects

**Resources:**
#### [Hands on Deep Learning for Games Ch3 - WGAN](https://github.com/PacktPublishing/Hands-On-Deep-Learning-for-Games/blob/master/Chapter03/Chapter_3/Chapter_3_3.py)

## Day 3: 
**Today's Progress:**
##### Coding: 
- Managed to get pytorch installed on my Windows 10 system
- Ran a DCGAN to generate fake celebrity faces using torch and my personal GPU
- Ran a CGAN successfully using the colab notebook environment provided by Google

**Link to code:** 

(see 'Resources' below; change batch size from 32 to 64)

**Results / Thoughts:**

![dcgan celeba results](https://raw.githubusercontent.com/aztecman/21_DAYS_OF_GANS/master/day3_celeba_fix.png)
![cgan mnist results](https://raw.githubusercontent.com/aztecman/21_DAYS_OF_GANS/master/day3_cgan_mnist.png)

##### Wow, today was an incredible success. I didn't make much in the way of changes to the code, except raising the batch size for the CGAN from 32 to 64. Some of the faces generated by the partially trained network are particularly interesting.

**Future Work:**
- Generate some magic cards - one approach would be to find faces in the cards and insert them into the celebrities dataset
- Learn the fundamentals of Pytorch.
- Run a CGAN in Pytorch
- Generate animals with a CGAN
- Generate galaxies with a CGAN
- Generate flowers with a CGAN
- Run an ACGAN in Pytorch (also in keras)

**Resources:**
#### [DCGAN PYTORCH TUTORIAL](https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html)
#### [GANs in Action Chapter 8](https://colab.research.google.com/github/GANs-in-Action/gans-in-action/blob/master/chapter-8/Chapter_8_CGAN.ipynb)

## Day 4:
**Today's Progress:**
##### Coding
- Successfully ran a conditional GAN on cifar10

**Link to code:** 

(see 'Resources' below; change batch size from 16 to 64, as well as increased the number of epochs from 20 to 200)

**Results / Thoughts:**

![results A](https://raw.githubusercontent.com/aztecman/21_DAYS_OF_GANS/master/day4_A.png)
![results B](https://raw.githubusercontent.com/aztecman/21_DAYS_OF_GANS/master/day4_B.png)

##### While I would hesitate to call them realistic, today's results are as good as I could reasonably hope to achieve. It was peculiar to watch the training, as I would not expect to see mode collapse between different classes, as I observed. I'm curious if this would manifest similarly in an ACGAN.

**Future Work:**
- Generate textures for a 3d model using a GAN (might require a research project)
- Generate some scifi art with a GAN

**Resources:**
#### [Training a Conditional DC-GAN on CIFAR-10 by Utkarsh Desai](https://medium.com/@utk.is.here/training-a-conditional-dc-gan-on-cifar-10-fce88395d610)
#### [Code for blogpost](https://colab.research.google.com/github/utkd/gans/blob/master/cifar10cgan.ipynb)

## Day 5:
**Today's Progress:**
##### Coding
- Tried to run a cycleGAN and completely failed
- Loaded up some pretrained GANs on tensorflow hub

**Link to code:** 

(see 'Resources' below)

**Results / Thoughts:**

[TODO: upload results]

##### I rediscovered the [Galaxy Zoo Data set](https://data.galaxyzoo.org/) today. Other than that, nothing spectacular occured.

**Future Work:**
- Perform Super-resolution with a GAN
- Practice breaking the structure of [Lucid/misc/GL](https://github.com/tensorflow/lucid/tree/master/lucid/misc/gl) in order to tease appart how to go about projecting from 2d onto a 3d object's texture-map.
- Migrate the high-grade DCGAN from tensorflow 2.0 backward to prior version (so it works on my Windows pc).
- Find a version of Pix2Pix that will run on my Windows PC.
- Learn to save checkpoints and resume from them in keras/tensorflow as well as pytorch.
- Learn to interpolate (presumably by manipulating the noise fed to the generator)
- Explore disentangled representations
- Explore Patch-GAN

**Resources:**
#### [Compare GAN modules (with tf hub)](https://colab.research.google.com/github/google/compare_gan/blob/v2/compare_gan/src/tfhub_models.ipynb)

## Day 6:
**Today's Progress:**
##### Reading / Studying code
- I spent some time today looking through Lucid examples on feature visualization and style transfer for 3D models. 

**Results / Thoughts:**

##### Although I didn't accomplish any coding today, I feel satisfied in becoming better aquainted with with texture synthesis for 3d models.

**Future Work:**
- Generate some simple 2D textures
- Study linear algebra
- Study OpenGL

**Resources:**
#### [Texture Synthesis on Papers with Code](https://paperswithcode.com/task/texture-synthesis)
#### [Immersive Math: Linear Algebra](http://immersivemath.com/ila/index.html)
#### [OpenGL Tutorial](http://www.opengl-tutorial.org/)

## Day 7:
**Today's Progress:**
##### coding
- Modified an ACGAN to run in colab

**Link to code:** 

[TODO add colab notebook]

**Results / Thoughts:**

[TODO add images]

##### I borrowed an ACGAN example from the book Advanced Deep Learning with Keras. After a few minutes of training, it became evident that the 40,000 epochs (chosen by the author) would result in a 33 hour runtime for my notebook. Since colab notebooks run for a maximum of 12 hours at a time, I knew that I would have to decrease the number of epochs. I settled on 2500 epochs. The results are not very pleasing. Aside from that, I spent some time to familiarize myself with OpenGL.

**Future Work:**
- Work my way through the 3rd Chapter of OpenGL's tutorial
- Begin to explore PyOpenGL
- Study tensorflow
- Try out Text based GANs (Text-to-Image)

**Resources:**
#### [ACGAN - Advanced Deep Learning With Keras](https://github.com/PacktPublishing/Advanced-Deep-Learning-with-Keras/blob/master/chapter5-improved-gan/acgan-mnist-5.3.1.py)
#### [Open Gl Tutorial](http://www.opengl-tutorial.org)
#### [Introduction to Tensorflow for AI, ML, and Deep Learning](https://www.coursera.org/learn/introduction-tensorflow/)

## Day 8:
**Today's Progress:**
##### Reading
- I read several pieces by Connor Shorten, including one that I found very interesting, on Self-Supervised GANs.
##### Video Learning
- I watched 18 short videos talking about the math behind GANs and other NN architectures
##### Coding
- Tried out 'Neural Painter'

**Link to code:** 

[see 'Resources']

**Results / Thoughts:**

[TODO add images]

##### I'm very pleased with these results. After several hours of training I was rewarded with a video of the training session. If you check out the author's github (see 'Resources' below), they have quite a few colab notebooks explaining different aspects of their approach. I find this effort toward reproducability very inspiring.

**Future Work:**
- explore the various aspects of Neural Painters in depth
- explore Self Supervised GANs in greater depth

**Resources:**
#### [Neural Painters on Github](https://github.com/reiinakano/neural-painters)
#### [Connor Shorten on Medium](https://medium.com/@connorshorten300)
#### [Henry AI Labs on Youtube](https://www.youtube.com/channel/UCHB9VepY6kYvZjj0Bgxnpbw/videos)

## Day 9:
**Today's Progress:**
##### Reading
- I read a few more articles by Connor Shorten.
##### Writing
- I began a rough draft of an article themed on top GANs of 2019
##### Coding
- Tried out Gene Kogan's pretrained bigGAN demo
- I managed to get through the 2nd and 3rd chapters of OpenGL basics tutorial (in c++)

**Link to code:** 

[see 'Resources']

**Results / Thoughts:**

[TODO add images]

##### Today's noodling was quite a bit of fun. I produced far more images and videos than I will bother to share here. It was interesting to see how similar sets of images were produced based on a common noise vector. 

**Future Work:**
- read the bigGAN paper
- read the progressive GAN paper
- read the stack-GAN paper

**Resources:**
#### [Gene Kogan's pretrained GAN Demo](https://colab.research.google.com/drive/1rqDwIddy0eunhhV8yrznG4SNiB5XWFJJ)

