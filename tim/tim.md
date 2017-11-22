<section data-background="tim/michal-lomza-338227.jpg">
<div align="right"><font color="black">

### Magical Methods:
####Using Topic Models in Digital Humanities' Research

#### Shawn Graham, History
####shawngraham.github.io
http://j.mp/TIM-11-22


---
<section data-background="tim/vimes.jpg">
<div align="left">
<br><br><br><br><br><br><Br><br><br><br><br>
>That's why I don't like magic, captain.  'Cos it's magic.  You can't ask questions, it's magic.  It doesn't explain anything, it's magic... <Br><br> That's what I don't like about magic, it does everything by magic! <br>- Sam Vimes (Thud, Terry Pratchett)

</div>
</section>
Note:
the problem with magic - sam vimes. many folks in humanities feel similarly about digital methods. it is a black box: and because it appears magical, un-interrogateable, it can be the bogeyman, the focus of all our worst fears.

---

** The Plan **

+ the problems of historians
+ my data are _this big!_
+ the dangers of borrowing
+ how topic models work (ish)
+ fun things to do with this magical method
+ where we go from here

---
<section data-background="tim/neil-cooper-318875.jpg">

**So many books.**

**So little time.**
</section>
Note:
why historians interested in large scale approaches to text - roy rosenzweig. scarcity versus abundance. but a big issue: historians pretend that they aren't using digital methods. milligan, illusory order. so they sneak a little magic in, but pretend it's not there, and that way, they can pretend that it doesn't have theoretical implications, that method is theory free, and that they certainly don't have to think about the underlying networks of power and resources that makes this research possible. or to think about keyword search works. or the errors of OCR - Cordell, Quoth the Raven; Shawville Equity

---
<section data-background="tim/troy_pba_pottery_tent.jpg">
</section>
Note:
different sized corpora that historians deal with. relativity of ‘big’. historians not the only ones who pretend like this. 'big' is a moving goalpost. Shopify 'cotton socks' story. Bigger, faster, theory-free, everything will percolate up in the associations and correlations... we've been here before

---

The Spectre of Cliometrics

Note:
an approach associated with economic historians of the late 70s, early 80s. i'm not a historian, not really, but it looks to me to have been paralleled in archaeology with a certain kind of processual thinking where MOAR DATA and frequentist statistics would give us The Answer. Historians reacted against this - since many of them lacked even basic statistical training, such that there are very few economic historians in history departments these days.

---


<div align="left">
#### The world of information is more Gothic <br>than its believers believe, <br>because it is ghostly, <br>silhouette-like, <br>deprived of human sentience
<br>
#### Arnold Weinstein
</div>
<section data-background="uclbigdatagothic/saturn-eating-child.jpg"></section>

Note:
These two reactions - the rejection and wholehearted adoption of magical methods seem to me to be two sides of the same coin. I like the phrase 'big data gothic' to describe this.

---

####[The Gothic] aimed to produce emotionally vertiginous shocks and thrills;<br> sensations of any kind, in fact, so long as they put the viewing subject - the 'Self' - at the centre of the experience.
<br>

Richard Marggraf Turley

---

#### "The goal<br> was to <br>overwhelm <br>the senses,<br> to annihilate<br> 'Self'."
<section data-background="tim/wanderer.jpg">
</section>

Note:
vista: terrifies us in its sublime vision. I am spending time describing all of this to give us a bit of a framework for using all these magical methods productively. If you ever find yourself shrugging and blaming The Algorithm, that's big data gothic; if you find yourself enthusing about the results to the degree that you're able to fit any explanation around the results and make it sound plausible - that's big data gothic.


---

The geek in me thrills at the ability to read, and make sense of, thousands of documents at a time.

The pessimist in me worries about what off-loading meaning-making to an algorithm does to our sense of humanity.

Note:
we have to understand what the method does well enough to know when what we're seeing is an artefact of how we've shaped the data, how we've put our thumb on the scales. We are taught every day to accept the outcome of the algorithm as neutral, divine even - "I'm sorry sir but the computer says..."

---
<section data-background="tim/chris-barbalis-186421.jpg">
<div align="right"><font color="black">
>**...said the archaeologist,<Br> educated in earth-sciences,<br> who hides in the history department, masquerading as a digital humanist.**
</font></div>
<section>


Note:
background of archaes re computation - idea that we’ve this dual nature, science & humanities; sci method w/ humanistic interp. I feel that while I am probably a C-List digital humanities guy, I've lived in the interstices of different schools of thought that what I'm saying here contains a bit of Truth that'll help other people make more informed use of these magical methods. But I would say that, wouldn't I?


---

_cum grano salis_

You Have Been Warned

---

The Critical Difference:

Justification versus Discovery

Note:
archaeology had its moment about 20 odd years ago re computation: computation was there to *prove* something! it was all hypothesis testing, sampling strategies, models and the goal: 'mid range theory', something that would bridge the fragmentary evidence to the grand stories about the past we wanted to tell. the archaeology wars were bitter, divisive. there are still the true believers out there, but most now recognize that you do all of these things in a framework of interpretation, that the computation doesn't *prove* anything, in and of itself. instead, it helps tell better v worse stories. the DH versionn of this summed up in this lovely aphorism of trevor owens.
and mining - problems and assumptions of data mining as used by humanists. note these are literary people; archaeos sorted this out a while ago https://academic.oup.com/dsh/article/23/4/409/1036906. So, let's actually get to the meat and potatoes: what is topic modeling, what does it do, and why should I care?

---
<br><b><Br><br><br><Br><br><br><br>
## Topic Models are for Discovery
<section data-background="tim/teddy-kelley-98551.jpg">
</section>
---
[![A Brief Video on Topic Models](https://img.youtube.com/vi/gN2x_KjJI1o/0.jpg)](https://www.youtube.com/watch?v=gN2x_KjJI1o)

Note:
how TM works - informal description

--

![gettysburg](tim/gettysburg.png)
Find, and count, the "war" words, and the "governance" words

[then we'll go to Voyant Tools](http://voyant-tools.org/?corpus=985b82cc0fc06a1b6b43e06a21838d9f&view=Topics)


Note:
TM by hand exercise. 293 unique words

--

![ted underwood](https://tedunderwood.files.wordpress.com/2012/04/ldaformula.png)

Note:
"Suppose we knew which topic produced every word in the collection, except for this one word in document D. The word happens to be “lead,” which we’ll call word type W. How are we going to decide whether this occurrence of W belongs to topic Z?
We can’t know for sure. But one way to guess is to consider two questions. A) How often does “lead” appear in topic Z elsewhere? If “lead” often occurs in discussions of Z, then this instance of “lead” might belong to Z as well. But a word can be common in more than one topic. And we don’t want to assign “lead” to a topic about leadership if this document is mostly about heavy metal contamination. So we also need to consider B) How common is topic Z in the rest of this document?
Here’s what we’ll do. For each possible topic Z, we’ll multiply the frequency of this word type W in Z by the number of other words in document D that already belong to Z. The result will represent the probability that this word came from Z. "
-the underwear example, re bayes

--

- topics have a distribution over words
- documents have a distribution over topics
- since we don't know the number of topics, we guess
- the model uses that guess to estimate the probabilities
- you can end up with a model and estimated likelihood that its a good model

[you could do worse than to look at the Wikipedia page on LDA](https://en.wikipedia.org/wiki/Latent_Dirichlet_allocation)

Note:
mathematics of how TM works

---

# Topic Models I Have Known

Note:
interesting uses of TM for historians


---
[A Distant Read of the Day of Archaeology](https://github.com/benmarwick/dayofarchaeology)
![](https://github.com/benmarwick/dayofarchaeology/raw/master/figures/topicdiffs.png)
---

[20 000 articles over 75 years of scholarship](http://graeworks.net/digitalarchae/20000/)
![](tim/20000.png)

---

Portable Antiquities Scheme ~ 2 million records

![](tim/excelheatmap.png)

---

You can even listen to topic models

[![John Adams 20](https://img.youtube.com/vi/ikqRXtI3JeA/0.jpg)](https://www.youtube.com/watch?v=ikqRXtI3JeA)

---

Historians most often use topic models for data with a strong chronological element - diaries, newspapers - to understand change over time, and to challenge periodization. [Mining the Dispatch](http://dsl.richmond.edu/dispatch/Topics)

![dispatch](tim/dispatch.png)

Note:
dispatch; diary of what’s her name


---
<section data-background="tim/pompeii.jpg">
[Reconstructing Pompeian Households, Mimno](https://mimno.infosci.cornell.edu/papers/pompeii.pdf)
</section>
Note:
mimno, in pompeian houses


---

![](tim/genes.png)

Note:
uses of TM in other fields

---

[Toronto Historical Plaques](http://themacroscope.org/interactive/toplaques/) extends topic models over space as well.

Note:
other cool text analysis
tools like word vectors

---

[The Lives of 8000 Canadians](http://themacroscope.org/interactive/dcbtopicnet/)

---

![bonetrade](tim/bonetradesampler.png)

Note:
dehumanizing numbers, trade that literally commodifies humans, taking place on a platform rife with bots... the different kinds of analysis we tried, including word-embeddings (explain) and text-reuse.

---

![](http://intarch.ac.uk/journal/issue45/5/images/figure4th.png)

    [8] 'sale real osteology bone medical oddities sold shipping worldwide specimen'
    [19] 'bones anatomy skeleton medical death museum medicine tattoo doctor photo'
    [17] 'tribal asmat bone dayak tribalart kapala tibetan trophy tin headhunter'

Note:
this is one cluster of very closely related topics. the close association of topics clearly connected with buying and selling, and topics related to trophy skulls and other indigenous ethnographic materials. While a post might not necessarily mention a trophy skull being bought and sold, the patterns of discourse are very similar. These materials are not being discussed with respect, but as commodities. And topic modeling reveals the subtle sorts of discourses - habits of thought that we unconsciously draw on given our own particular contexts - that make buying and selling human remains possible. In this way I come full circle back to my earlier concerns about big data context.

---

<section data-background="tim/granny_weatherwax_by_daoyiliu-d8h0z0i.jpg">
<div align="left">
<br><br>"It's a lot more complicated than that--"<br><br>

"No. It ain't. When people say things are a lot more <br>
complicated than that, they means they're getting worried <br>
that they won't like the truth. People as things, <br>
that's where it starts."<br><br>

"Oh, I'm sure there are worse crimes--"<br><br>

"But they starts with thinking about people as things..."<br><br>

Terry Pratchett, _Carpe Jugulum_
</div></section>


Note:
it's useful to reflect on Granny, especially with regard to how historians use digital history stuff - that we fall into the trap I discussed at the beginning, of being swept away by the terror of the digital gothic, and that we forget that there are humans behind all of this.

---

### magical methods

- require each step be articulated in relation to the research question
  - partly because methods borrowed from other disciplines
  - partly to justify
  - mostly for discovery


Note:
so this is how we guard about getting carried away by the magic.
partly also b/c a gap has emerged b/t how historians are assumed to work (in archives, etc) and what they’re actually doing, ie pretending to have read the entire newspaper in context and selecting the relevant info versus actual: illusory order


---

dh deliberately transforms sources into data,

and simplifies data into models

Note:
thus datasets, and data models, and their creation, need to be published and critically reviewed, as much or more so than the stories we tell from them!

---

![](tim/xkcd.jpg)

---

> It doesn't stop being magic just because you know how it works. - T. Pratchett

_Thank You_

[shawngraham.github.io](http://shawngraham.github.io)

Note:
conclusion
magic methods of dh still need to be carefully grounded, and understood in the context of the method’s own historiographical trajectory.

---

Let's get our hands dirty.

- download [the topic modeling tool](https://senderle.github.io/topic-modeling-tool/documentation/2017/01/06/quickstart.html)
- download and extract the file and folder from [this zipfile - John Adam's Diary](https://www.dropbox.com/s/x40a367isiz9ipp/TM-Workshop-Archive.zip?dl=0)
- remove the 'ds_store' file if it's present

---
- feed the tool the Diary
- set the metadata with the options

---
- What can you learn about John Adams from this distant read of his diary?
- What does the output in the console tell you?

---

- How do the topics change over time?
- What difference to your reading does having more or fewer topics make?

---

- How does setting the option, 'divide input into n-word chunks' make a difference? Try n = 2, n = 3, n = 4
- How might you use this tool in your own research?

---
## More Things To read

[Blei et al](http://jmlr.csail.mit.edu/papers/volume3/blei03a/blei03a.pdf)

[Ted Underwood](https://tedunderwood.com/2012/04/07/topic-modeling-made-just-simple-enough/)

[Scott Weingart](http://www.scottbot.net/HIAL/index.html@p=19113.html)

[Matt Jockers](http://www.matthewjockers.net/2011/09/29/the-lda-buffet-is-now-open-or-latent-dirichlet-allocation-for-english-majors/)

[Clay Templeton](http://mith.umd.edu/topic-modeling-in-the-humanities-an-overview/)

[Miriam Posner](http://miriamposner.com/blog/very-basic-strategies-for-interpreting-results-from-the-topic-modeling-tool/)

---

## Photo/Art Credits

+ Paul Kidby
+ Neil Cooper, unsplash.com
+ Projekt Troia. Photographer Gebhard Bieg; with permission.
+ Chris Barbalis, unsplash.com
+ Teddy Kelley, unsplash.com
+ daoyiliu
+ xkcd
