### Investigating the Rhetoric
## of the
# Online Trade in Human Remains

Shawn Graham [@electricarchaeo](http://twitter.com/electricarchaeo) & Damien Huffer [@DamienHuffer](http://twitter.com/DamienHuffer)

follow along at http://j.mp/bonetrade

---
![](saa2018/mosaic.jpg)

when people want to buy bones, where do they go?

when people want to sell bones, where do they go?

Note:

given that much of this trade is morally dubious and legally in various grey zones

_how_ do they negotiate this sale?

---

> 'I have a pile of teeny human skull scraps laying around. Due to etsys rules i cannot sell human bone or make a listing but id love to do custom orders for anyone interested in a pendant, ring, etc made from a human skull fragment. Dm me! #bone #bones #skull #humanbone #humanskull #fragment #skullfragment #oddities #oddity.'
https://www.instagram.com/p/znHyR7AbXS/

![](saa2018/skull-for-sale.jpg)

Note:
Not everyone is as bold as this. Most are aware that their _posts_ can be searched (ie key-word searching), and so rely on more subtle cues

---

On Instagram alone _where dollar values were named_

total amounted to approximately $190,000

The value of private sales cannot of course be known

---

## Cultural impact:

no.s of followers, following of _just those accounts that name a price_

a network with 138,014 individuals connected by 172,208 links

Note:
association with taxidermy, tattoo parlours - do i still have that cardiff photo?
three broad groupings: specialists explicitly interested in bones; generalists who follow the bones but also other things; and people who don't post pictures themselves but follow the bone accounts

---

![](saa2018/screenshot-belgian-video.png)

Note:
video of man in Belgium degreasing a skull. Likely source for such a skull? WW1 battlefield. He's preparing it for cutting into an exploded view.

desecration of ww2 battleship wrecks - steel is pre 1945, so different atomic signature thus valuable; bones collected, given to the boss... what happens to them?

---

![](saa2018/8-100-1-SP.png)
![](saa2017/ata.png)

Note:

'exotic fetishizing' of the dead, and esp. the non-western dead

especially with the shutting down of collections built at the start of the 20th century tied up with that 'scientific racism'

Ata mummy - promotion of pseudoscience and racism to broader culture

---

## Understanding the trade in human remains matters.

---

How do we deal with it?

Note:
Part of the problem is that not all of this is _illegal_. approaches and issues are of a part with broader trade in antiquities.

broader trade tends to focus on the auction houses and the big collectors; smaller objects, ebay, etc do not attract as much attention

but the techniques developed to deal with these smaller items could be of significance for studying the broader trade, and the penetration of archaeological consciousness into the broader publics

---

## digital archaeology
### meets
## digital humanities

Note:

digital humanities approaches to data mining try to understand the contextual significance of what has been extracted

in our work, we have in the first instance scraped ~ 13 000 posts from one calendar year on Instagram (one of many places where human remains are traded); some posts were caught in the trawl as far back as 2013

---
![](saa2018/dendro-topics.png)


    [8] 'sale real osteology bone medical oddities sold shipping worldwide specimen'
    [19] 'bones anatomy skeleton medical death museum medicine tattoo doctor photo'
    [17] 'tribal asmat bone dayak tribalart kapala tibetan trophy tin headhunter'

Note:

we focussed on the _language_ the posts, building topic models and word vectors to understand some of the rhetorical constructions of buying and selling human Remains

---

![](saa2018/vectors.png)

Note:
Exploring the vector space defined by binary pairs, 'good'-'bad', 'for sale'-'not for sale’. Hints of various dynamics at play can be viewed in contrasting, but related, terms, e.g. as with ‘acrylic painting’ falling in negative space and ‘skull decor’ falling in positive space. This might be a glimpse into the taste or aesthetic of those who create skull-related art, which may be important for understanding what creates the taste and demand for human remains themselves.

literal posts, 'human skulls for sale' do exist; but often the language is coded, more oblique, and seems to depend on the composition of the image itself to signal something for sale

---

## so that's what we've done

### here's what we're doing

Note:
our current research is looking at the composition of the images themselves, computationally. There are too many images to do the classificatory work ourselves. Some approaches to these kind of image classification or determinations of similarity employ 'human' computers like the Amazon Mechanical Turk service. There are serious ethical issues with employing that kind of labour on this material.

---

![](https://ujwlkarn.files.wordpress.com/2016/08/screen-shot-2016-08-07-at-4-59-29-pm.png?w=1493)

(an oft-copied diagram of the structure of a CNN)

Note:

instead, we are using a class of machine learning called 'convolutional neural networks' that build up a numerical representation of the features within an image. Such neural networks are built by analogy to how the human brain processes images. One of the largest and most accessible neural networks is Google's Inception v3 model.

---

![](https://4.bp.blogspot.com/-TMOLlkJBxms/Vt3HQXpE2cI/AAAAAAAAA8E/7X7XRFOY6Xo/s1600/image03.png)

(Google's very own diagram. Helpful, eh?)

Note:

normally, one would feed an image to Inception, and it would recognize the particular pattern of features as being similar to others it 'knows', and it would spit out a label for what is in the image.

---
<section data-background="saa2018/duhaime.png">

Note:
if however we stop the process just before the image labelling, we can use the vector representations of our images to compute similarities (the full details will be in our forthcoming JCAA paper). We are completely indebted to Douglas Duhaime and colleagues for clearly explicating and coding how this can be done.

---

![](saa2018/8-98-1-SP.png)

Note:

disclaimer: These images are deliberately distant so that we can discuss the structure of what we're finding but not put the dead on display.

This is where we are at right now. After turning all of the images into vector representations, we use some statistical magic (t-sne and affinity clustering propagation) to understand the structure of visual similarity in the posts. The clustering algorithm identifies 'exemplar' images for each of the clusters that it finds.

---

<section data-background="saa2018/8-97-1-SP.png">

Note:

We examine these exemplars - in our corpus, that's 84 images - by eye to work out what it is that the computer is 'seeing', comparing and correlating with our data mining of the text of posts themselves..

---

<section data-background="saa2018/8-99-1-SP.png">

Note:

So far, it appears that the computer can discriminate skulls for sale by their arrangement on the shelf. Items for sale are arranged in ways that mimic 'popular' understandings of museology - glass cabinets with skulls arranged by size for instance.

Other clusters have been photographed square to the face, and largely fill the frame, and the associated language is largely of 'look at my collection' and 'look what i just gave away', perhaps signaling in other images that these materials could also be 'given away' - for a price. Another cluster positions the skulls such that they are turned slightly to the left; associated texts here clearly indicate something for sale.

This initial experiment does seem to support the idea that items for sale are displayed in ways that are discernible to the machine, and so, the machine can be taught to trawl other bodies of data for more evidence of the trade in human remains. The machine directs our attention to the framing of photographs, and the relationship of the human remains to other elements within the photograph. Exhibition design – rows of objects in cases on display – are recreated here. The interplay of foreground and background also seems to be important. Photos composed to show off a collection might also be subtly signaling that the item might also be for sale. These signals could be isolated, and used to train further iterations of a CNN, allowing a researcher to scale up their investigation. We intend to cross-reference this data with the network of followers and followed, to see how these visual clusters play out across networks of influence and on other platforms aside from Instagram.

---

## It's still early days.

Note:

This work is in its early stages. Despite being trained on a very generic corpus of images, Inception v3 seems to be a very powerful model for pulling out some of the visual rhetoric of display. If we train a model ourselves explicitly on archaeological materials, can we identify automatically at scale legal from illegal sales? ethical from non-ethical displays of remains? can we build an archaeo-crawler that would search these images, posts, and peoples out? would such a use be ethical? could one work out likely source peoples to whom these remains belong? given the use of computer vision for surveillance and social control, to what degree is our work dangerous and complicit? How do we ethically use computation to combat the trade?

---

### thank you
