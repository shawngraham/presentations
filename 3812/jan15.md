
### housekeeping

follow along at [http://j.mp/2DAg3hg](http://j.mp/2DAg3hg)

---

### http://jonudell.net/h/facet.html

![](3812/udell.png)

---

![](3812/3812-topics.png)

---

![](3812/keywords-user.png)

---

![](3812/bigrams-date.png)

---

<section data-background="3812/jan15-1.JPG">

### Intro to Photogrammetry

---

+ part of a suite of approaches related to geomatics, computer vision
+ the kind we now see in apps & getting more user-friendly is _structure from motion_

---

This kind of thing:

![](http://www.spatialhumanities.de/typo3temp/pics/TLS_Terrestrial_Laser_scanner_Spatial_Humanities_1e016bb648.png)

---

to this kind of thing:

![](https://hackadaycom.files.wordpress.com/2013/09/rubicon.jpg?w=800&h=483)

---

to this kind of thing:

![](https://3dscanexpert.com/wp-content/uploads/bevel-3d-scanner-review-package-1500x810.x92699.jpg)

...which doesn't really work very well at all...

---

...all you really need is just a camera...

---

### Some Things I've Tried

---

[Pop-Up Book, FYSM1405](https://electricarchaeologist.files.wordpress.com/2012/05/fysm1405_cover_and_book_2.pdf)

[model](https://p3d.in/zwPEM/spin)

---

![](3812/pompeii-book.jpeg)

Built from [this video](https://youtu.be/EfeSZ7KTVnQ)

---

CSTM project on the Air Canada Collection

- view with [Augment](https://play.google.com/store/apps/details?id=com.ar.augment&hl=en)

- [download the book here](http://5702x.graeworks.net/wp-content/uploads/2014/04/version-for-web-april112014-2.pdf). 

It's been a while since I checked this. It might not work anymore. 

---

Here's [one of the models](https://sketchfab.com/models/e24007259dda4d08865838ddc5addcf4)
<div class="sketchfab-embed-wrapper"><iframe width="640" height="480" src="https://sketchfab.com/models/e24007259dda4d08865838ddc5addcf4/embed" frameborder="0" allowvr allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true" onmousewheel=""></iframe>

<p style="font-size: 13px; font-weight: normal; margin: 5px; color: #4A4A4A;">
    <a href="https://sketchfab.com/models/e24007259dda4d08865838ddc5addcf4?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank" style="font-weight: bold; color: #1CAAD9;">Air Canada Stewardess&#39; Dress, CSTM</a>
    by <a href="https://sketchfab.com/electricarchaeo?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank" style="font-weight: bold; color: #1CAAD9;">electricarchaeo</a>
    on <a href="https://sketchfab.com?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank" style="font-weight: bold; color: #1CAAD9;">Sketchfab</a>
</p>
</div>

---

<section data-background="https://electricarchaeologist.files.wordpress.com/2015/07/m1.jpg">

# The Diary In The Attic

>Shawn dusted off the old diary. 'Smells of mould', he thought, as he flipped through the pages.'Hmmph. Somebody was pretty careless with their coffee. <br> I think it's coffee. <br> Hmm. <br> Doesn't smell like coffee. <br> What the hell... Damn, this isn't coffee.

Shawn cast about him, looking for the android digital spectralscope he kept handy for such occasions. Getting out his phone, he loaded the spectralscope up and, taking a safe position two or three feet away, gazed through it at the pages of the diary.

> My god...it's full of...

[download apk](https://www.dropbox.com/s/pbj9tng5t2z7me1/nilediary2.apk?dl=0)

[download diary](https://www.dropbox.com/s/ygivh6xkof935xy/nilediary.pdf?dl=0)

---

[My Sketchfab Account](https://sketchfab.com/electricarchaeo)

---

## Ok. So how do _we_ do any of that?

---

English Heritage: [Photogrammetric Applications for Cultural Heritage](https://historicengland.org.uk/images-books/publications/photogrammetric-applications-for-cultural-heritage/)
---

## Basic Principles

- image capture
- image matching
- dense point cloud generation

---

## Basic Principles Continued

- secondary product generation
- analysis / presentation

---

![](3812/jan15-1.JPG)

---

![](3812/jan15-2.JPG)

---

![](3812/jan15-3.JPG)

---

![](3812/jan15-4.jpg)

---

![](3812/jan15-5.JPG)

---

![](3812/jan15-6.JPG)

---

![](3812/jan15-7.JPG)

---

### chief ray & principle of intersection, collinearity

- knowing the 'interior and exterior' orientation of the camera - its internal arrangements, including lens distortion, focal length and so on from the metadata bundled with the image, allows software to work out the position of the camera viz points of overlap in the images
- the intersection of rays then allows us to work out the location of these points in space
- resulting point cloud has an arbitrary scale and coordinate frame (ways around this)

---

### sfm process
- identifies control points that are visible in multiple images (default in agisoft photoscan is 40 000 _per image_)
- best control points are then matched
- then triangulation (more or less) to work out the relative position & orientation of every image

this is the sparse reconstruction

---

### now dense reconstruction

- repeats the process above but for all possible control points
- a 'triangulated irregular network' TIN is generated, a mesh, onto which textures can be mapped using regular graphics software

---

### then what?

- download to your computer; clean up with ie [meshlab](http://www.meshlab.net/) or [blender](https://www.blender.org/)

---

- you can also use meshlab to mash up your model with something else

---

Sources of other models:

- [sketchfab.com](http://sketchfab.com)
- [thingverse](https://www.thingiverse.com/)
- [smithsonian](https://3d.si.edu/browser/) (hit the info button on a model for the download options)

---

- upload to Sketchfab for sharing, hosting

---

## Wednesday:

- I'll be in the department, in the Underhill Resource Room (go to the foyer, turn left, left again) to show folks how to use Agisoft Photoscan (where you take photos with your own camera and then process them, no app)
- You can join me there, or, you can head out onto campus, into the city, or one of the museums, and try some 3d photogrammetry on your own.

