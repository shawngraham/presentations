# Intro to Photogrammetry

---

+ part of a suite of approaches related to geomatics, computer vision
+ the kind we now see in apps & getting more userfriendly is _structure from motion_

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

--

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
