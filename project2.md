Project 2:
Due: Wednesday October 8, Noon.
Teaming: You can do this project in team of 1, 2, or 3.

Please submit your blog post here: [submission link](https://docs.google.com/forms/d/e/1FAIpQLSdwxPTHp_a1A3iIGpE5SyrRAwf5NgfL7_tHO2Ts372YWgFcyg/viewform?usp=sharing&ouid=113271021017255380934f)

You can make a blog for yourself and post pages from it via the GWU blog service: https://blogs.gwu.edu/, 
or use public services like github, wordpress, etc.  

The goal of this project is to experiment with Vision Language Models, and to give you intuition about current methods to compute embeddings.  In particular you are to explore one of the biggest challenges in Visual Language Modelling, the "modality gap" between text and image embeddings.

My CLIP-Challange has two parts.  

PART 1:

First, here are 5 images:
- [https://images.pexels.com/photos/36744/agriculture-arable-clouds-countryside.jpg](https://images.pexels.com/photos/36744/agriculture-arable-clouds-countryside.jpg)
- [https://images.pexels.com/photos/825947/pexels-photo-825947.jpeg ](https://images.pexels.com/photos/825947/pexels-photo-825947.jpeg)
- [https://images.pexels.com/photos/34044163/pexels-photo-34044163.jpeg](https://images.pexels.com/photos/34044163/pexels-photo-34044163.jpeg)
- [https://live.staticflickr.com/840/43380549381_004601c7ac_h.jpg](https://live.staticflickr.com/840/43380549381_004601c7ac_h.jpg)
- [https://live.staticflickr.com/2404/2020522557_d1aa0a1066_k.jpg](https://live.staticflickr.com/2404/2020522557_d1aa0a1066_k.jpg) (license:https://www.flickr.com/photos/briandewitt/2020522557/in/photolist-qCDWts-9LFMUT-uHeyNi-5G6LRz-45xGXP-hLkdkM-2ycbEf-3cHUMg-7y6Xh1-5Jqww1-hLm2hS-8gL5G-3WhbG4-EueMH-pfSn6-5dqjEz-4wHaBE-D3Ns2D-pBCiS-MpCHB-csWvU5-G97A4-6ZpBm5-6agE6f-5AGqd)

For each image, I want you to find the text that matches the image best.

- For each image I, Find the single word W that maximizes the cosine similarity (CLIP(I), CLIP(W)).
- For each image I, find the "simple structured caption" with 1 word so that minimizes the cosine similarity (CLIP(I), CLIP("A photo of a W")).
- For each image I, find the arbitrary caption C that minimizes the cosine similarity (CLIP(I), CLIP(C)).

You can do this with code (recommended), or with manual search (try a bunch of words yourself).  If you do it with manual search, you must tell the story about which word you tried, and what you learned (e.g. I tried "dog", and then I tried "puppy" and it gave a higher score so I thought I would keep trying more and more specific words.

PART 2
Find the pair of ("regular image",caption) (e.g. not an image of all white pixels or other super wierd artificial image), that gives the largest cosine similarity you can.  You are welcome to do this with manual search (again, explain all parts of your process), or with automated searches.  Those can be brute force or make use of online tools (e.g. you could generate the images and/or the captions).

Here is a [link to a Google Colab implementation](https://colab.research.google.com/drive/1o791kR0v08doy-xtY43OwHP-UTo1fAub?usp=sharing#scrollTo=22idPzo3aor9) of the most basic approach to compute CLIP features on an image and text.
