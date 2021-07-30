---
layout: post
title: 'MetalVis Tool'
---

If you're already familiar with the what and how of the MetalVis Tool, go wild and interactively explore thousands of actual band logos <a href="https://renecutura.eu/metalvis" target="_blank" rel="noopener"><span>**here**</span></a>! 

If you're not, Gerrit will try to explain and walk you through.

##### Let's skip the whole "What Is It?" part and take me straight to ...
- [How Can I Use It?](#what)
- [How Does It Work?](#work)

<a name="what"></a> 
#### What Is It?
In our paper, we try to explore the design space of Metal logos. To this end, Michael, Frank, and Rene have created a data-driven interactive webtool that allows users to explore, filter, and compare Metal logos based on certain characteristics such as **genre**, **color**, and **"image-likeness"**.

Of course, you could just google <a href="https://letmegooglethat.com/?q=Death+Metal+logos" target="_blank" rel="noopener"><span>Death Metal logos</span></a>, but this kind of search query usually ends up being unsatisfying at best; at worst, it gives a wrong impression of what Death Metal logos really look like. There are two problems: 

(1) A quick search result will only show some popular "Death Metal" logos. Note the quotation marks. I just did a quick search on Google and lo and behold there's the logo of **Obituary**, an influential Death Metal band from Tampa, Florida, but ... what is **Darkthrone**'s logo doing there? **Darkthrone** only ever put out one Death Metal album, and it wasn't even *that* great. (Hell, even the members of the band seems to think so.<sup>1</sup>) They're *infinitely* more famous for their contribution to Crust Punk -- come on, everyone knows that!<sup>2</sup> And who are those others bands even? In what (sub)genre do they fall: Death-Doom? Brutal Death? Melodic Death? Great! Now I have to google them, too. Who is Hga... Hgasohg--? Ah! <a href="https://letmegooglethat.com/?q=Who+are+Hellsong%3F" target="_blank" rel="noopener"><span>Hellsong</span></a>?

![Wait what](..\assets\img\projects\metalvis\screen.JPG)

(2) Google doesn't allow for tangible and intuitive comparative interaction. Let's say you first want to have an overview of some of the "proper" Blackened Death Metal logos out there; and then maybe you want to compare the design characteristics of these with, say, those of "traditional" Black Metal logos. The MetalVis Tool allows for just that.

<a name="work"></a> 
#### How Does It Work?
Now this is where things get technical -- *too* technical for me to explain. If you want to know the specifics, read the paper. 

Suffice here to say that Michael, Frank, and Rene have "scraped" openly available information of about 50,000 Metal bands from <a href="https://www.metal-archives.com/" target="_blank" rel="noopener"><span>Encyclopedia Metallum: The Metal Archives</span></a>, an online music database. For those unfamiliar with the Metal Archives, think of it as Wikipedia -- but for Heavy and Extreme Metal -- with editors having limiting and arbitrary notions about what counts as Metal and what doesn't. In that it's much like the SciVis community <sup>[citation needed]</sup>. Key data include band names, logos, genres, and lyrical themes. With all this information gathered and using sophisticated computer algorithms, they have built an interactive webtool called MetalVis. 

<a name="use"></a> 
#### How Can I Use It?
It's quite simple, really. First, you have to open yourself to the world of <a href="https://renecutura.eu/metalvis" target="_blank" rel="noopener"><span>**Metal logos**</span></a> by opening this web link. After you wait until the loading is complete, then you will see this screen -- a virtual cloud of logos.

![Metalvis](..\assets\img\projects\metalvis\screen2.JPG)

 If you zoom in, you'll see that this cloud is made up of thousands of logos -- to be a bit more precise, the number's close to five thousand!

![Zoom](..\assets\img\projects\metalvis\screen3.JPG)

On top there's a search box. Here, you can type in a specific band name. If the band is currently active, signed by a label, and part of the current sample of logos, a circle will appear in the cloud (you may have to drag the cloud around a bit to see it).<sup>3</sup>

![Search](..\assets\img\projects\metalvis\search.JPG)

You can zoom in on it and see it at a larger scale. You'll also notice some other band logos grouped around it. These logos are adjacent according to some given similarity criteria. To put it in simpler terms, the logos are grouped based on their attributes. Logos that are close together in the cloud should be similar according to some criteria.

Now if you click on the stack of dots in the top-right corner right next to where it says, "Gridified," you will see a pop-up window with four types of embeddings (ways of grouping the high-dimensional data and mapping it to a cloud). If you click on any of these, you'll see the cloud taking on a new shape (though it may take a while to load, depending on your PC). It's because the logos are now grouped according to another particular attribute or set thereof: respectively, image characteristics of the logo combined with band genres, only image characteristics, only band genres, and color.

![Embeddings](..\assets\img\projects\metalvis\screen5.jpg)

You may have already noticed that some of the logos overlap. It's because they are *that* similar -- according to the tool or embedding you used to sort the logos, at least. Some strange matches aside, the tool does a good job at showing which logos are similar in some way, and which ones are different. The less they have in common, be it visually or in terms of genre, the further they are separated from each other -- and vice versa.

To mitigate this overlap issue, you can choose to "gridify" the cloud. You do this by turning on the "gridified" button. By doing this the logos will be nicely separated from each other. However, you won't be able to see relative "closeness" or "farness" anymore.

![Embeddings](..\assets\img\projects\metalvis\gridified2.jpg)

One more thing needs mentioning; the tool offers some filtering options. In the left corner, you can toggle some switches to hide or unhide one or several genres (Heavy, Thrash, Death, and Black Metal); and in the right corner, you can click on the funnel symbol to bring up a popup window that provides various specific filtering options.

![Filters](..\assets\img\projects\metalvis\filter.JPG)

All right. Now you know everything you need to know to have fun with the tool! So, have fun!  


#### References and Other Notes
##### [1] B. Pilo. True Norwegian Black Metal: Nationalism and Authenticity. In: T.-M. Karjalainen, ed. *Sounds of Origin in Heavy Metal Music*, 43, 2018.
##### [2] D. Patterson. Black Metal: Evolution of the Cult, 207, 2013.
##### [3] This is not to "gatekeep," it was only done to keep things manageable in terms of numbers of bands and data points collected. Given the current scope of the project, we had to cut some things that we would've liked to have included. 
