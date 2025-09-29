Project 2:
Due: Wednesday October 8, Noon.
Teaming: You can do this project in team of 1, 2, or 3.

Please submit your blog post here: https://docs.google.com/forms/d/e/1FAIpQLSdwxPTHp_a1A3iIGpE5SyrRAwf5NgfL7_tHO2Ts372YWgFcyg/viewform?usp=sharing&ouid=113271021017255380934f

You can make a blog for yourself and post pages from it via the GWU blog service: https://blogs.gwu.edu/, 
or use public services like github, wordpress, etc.  

The goal of this project is to experiment with Vision Language Models, and to give you intuition about current methods to compute embeddings.  In particular you are to explore one of the biggest challenges in Visual Language Modelling, the "modality gap" between text and image embeddings.

My CLIP-Challange has two parts.  

First, here are 5 images.  For each image, I want you to find the text that matches the image best.

1a.  For each image I, Find the single word W that minimizes the cosine distance (CLIP(I), CLIP(W)).

1b.  For each image I, find the "simple structured caption" with 1 word so that minimizes the cosine distance (CLIP(I), CLIP("A photo of a W")).

1c.  For each image I, find the arbitrary caption C that minimizes the cosine distance (CLIP(I), CLIP(C)).

You can do this with code (recommended), or with manual search (try a bunch of words yourself).  If you do it with manual search, you must tell the story about which word you tried, and what you learned (e.g. I tried "dog", and then I tried "puppy" and it gave a higher score so I thought I would keep trying more and more specific words.

Part 2.
Find the pair of ("regular image",caption) (e.g. not an image of all white pixels or other super wierd artificial image), that gives the smallest cosine distance you can/

You are welcome to do this with manual search (again, explain all parts of your process), or with automated searches.  Those can be brute force or make use of online tools (e.g. you could generate the images and/or the captions).
