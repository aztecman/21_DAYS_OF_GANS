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

[TODO: add images]

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

[TODO upload ipynb, (or colab?)] (DCGAN)

[TODO link colab notebook]

**Results / Thoughts:**

[TODO: add images]

##### Wow, today was an incredible success. I didn't make much in the way of changes to the code, except raising the batch size for the CGAN from 32 to 64.

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
