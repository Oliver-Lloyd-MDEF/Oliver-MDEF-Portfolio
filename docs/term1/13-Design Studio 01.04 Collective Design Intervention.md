# Exploring Non-Human Intelligence

For the past 2 weeks we took part in our second design intervention for our Design Studio 01 module led by Jana & Roger. This time around we began a collective design intervention built out of our previous experiences, and interests. For this project my group and I had all expressed an interesting in using modern technology to better understand the world around us, and we wanted to explore the field of organic computing. We set out to learn as much as we could about the hidden world of plants, asking the question ***“How much could we learn if we actually listened?”*** 

---

### What did we do?

In the beginning, we returned to our collective design space in the MDEF classroom (room 301) and added in our new discoveries, interests and areas of exploration. After this we fell into various pockets of discussion around what we had found interesting, what we had discovered over the course of our first group and individual interventions and what directions this made us want to go into now. 

I joined this masters wanting to explore all sorts of strange and wonderful new areas of exploration that I wouldn’t normally be able to explore so I decided to try and explore an area that I’ve always found interesting but is vastly different from what I’m normally trained in, the field of interfacing technology with nature and moving towards organic computing. I ended up collaborating with my classmates Nicolo, Marius, Everardo, Jorge, and Albert, as we had all expressed an interest in this field.

We had no set roles throughout this project so far, as none of us had any prior knowledge on plant signalling, except Albert I suppose, who is an ecologist. Some of us had more experience with Arduino and coding so they took on those roles, but overall we all worked to help each other out.

When we started, we began with combing the internet for anything and everything we could find based on this topic ***(we found some cool stuff, I’ll link it at the bottom of this article)*** from computing research using mushrooms to making music with the electrical signals within plants. With one of the most interesting projects we’d come across demonstrating that you could use certain plants as analogue inputs and outputs. 

> ***one of the most interesting projects we’d come across demonstrating that you could use certain plants as analogue inputs and outputs.***
> 

What this bizarre sentence means is that you can effectively connect two plants together, use one as an input, and the other as an output. Meaning you can send a message between two plants! (for more on this crazy subject check out the TED talk on this subject linked [here](https://www.youtube.com/watch?feature=shared&v=pvBlSFVmoaw&ab_channel=TED))

So it turns out that our little green friends are actually much more sensitive than we give them credit for and they are able to process much more information than we can see. 

After discussing what we had found out together and mapping out each of our interests in a collaborative Miro board, we decided on a direction. 

---
<!--**insert pictures here of miro board mapping** -->
<img src="../images/10. Design Studio_Pulse Project/non human intelligence & Technology - Frame 1.jpg" alt="Miro Board mapping" style="border-radius: 5px;">
<figcaption> Our early Miro board mapping </figcaption>


---

We were going to try and receive, interpret and then eventually try and decode the electrical and chemical signals plants use to transmit information within themselves.

> **Imagine what we could learn if we really understood our ecology?**
> 

Luckily for us, some of these projects were open source and had freely shared everything they had learned on GitHub ***(bless the open source community).*** From these learnings we collected what we would need, a bunch of Arduino heart rate ECG monitors and the Arduino boards to control the whole system. 

Easy right? 

Not so much, first we tested the ECG sensors on ourselves and *no dice*. No matter how much we tried and what we changed, we just couldn’t get the contact pads to read the electrical signals produced by our own hearts (which is how these sensors work) let alone read the the much lower frequency signals created by the plants we were studying. 

<!-- **insert pictures here of ECG monitor testing** -->
<img src="../images/10. Design Studio_Pulse Project/ECG Testing.png" alt="ECG Testing" style="border-radius: 5px;">
<figcaption> A first test using the ECG monitors on ourselves </figcaption>

---

We eventually managed to read some sort of electrical spikes within an Orchid that we were studying and our excitement was over the moon! Though that excitement was shot down pretty quickly when we weren’t able to decipher if what we were reading was actual changes in electrical activity based on stimulus we were giving the plant or if it was just electrical noise and interference within the circuit itself. 

---
<!--
****************insert pictures here of ECG monitor hooked up to plant**************** -->
<div class="image-grid">
  <img src="../images/10. Design Studio_Pulse Project/ECG Orchid Test.png" class="grid-item" alt="Orchid ECG test">
  <img src="../images/10. Design Studio_Pulse Project/ECG Orchid Testing.gif" class="grid-item" alt="Orchid ECG Signal Test">

  <!-- Add more images as needed -->
</div>

<!-- CSS Styles -->
<style>
  /* Styles for the image grid container */
  .image-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr); /* Two columns */
    /*grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));*/ /*use this line of code to create a responsive grid that will place all images in one continuous row - each image will shrink accordignly*/
    grid-gap: 10px;
    /* Additional grid container styles can be added here */
  }

  /* Styles for individual grid items (images) */
  .grid-item {
    width: 100%;
    height: auto;
    object-fit: cover;
    border-radius: 5px; /* Add rounded corners to images */
    /* Additional styles for grid items can be added here */
  }
  /* Styles for portrait images */ /*apply this class to any portrait photo in a grid to crop it to landscape: class="grid-item portrait-image" */
  .portrait-image {
    object-position: center middle; /* Adjust this property to control the cropping of portrait images */
  }
</style>


---

**So back to square one. *Shit*.**

After a lot of work and research, we came across a project that had been using the same technology we were using to turn the electrical signals of plants into music using a MIDI synthesiser, lucky for us this project had been put up on GitHub (***[find out more here](https://github.com/electricityforprogress/BiodataSonificationBreadboardKit/blob/master/BiodataSonification_026_kit.ino))*** and we were able to reverse engineer the code they used. Reverse engineering this code, along with getting the ECG sensors to work properly while also calibrating them was probably the most challenging part of the process at this point in the project. From this we were able to build a custom circuit configuration using our Arduinos and ECGs to finally be able to read the signals properly. 

Then came the moment of truth…

We connected our trusty plant friend up to the ECG pads and plugged the other end into the circuit, a few moments passed as the system booted and looked for something in the ether. We held our breath for a moment as nothing seemed to be happening, hovering on the verge of failure once again when suddenly…spikes of activity! 

**SUCCESS!** 

To our shocked surprise it actually worked! We were reading the real and actual electrical signals within the plant! To test our theory we gently touched one of the leaves of our plant and shouted with joy as we watched the electrical signals spike as we touched it’s leaves. To make extra sure we then fed it a little bit of water and as the water started to sink into the roots of the plant, another series of spike in activity! 

We’d linked the signal monitoring program to a piece of software called Touch Designer,  which allows you to visualise pretty much any data input, so now we have some glowing spheres that grow larger or smaller based on peaks or troughs in the electrical activity — which I have to say looks pretty cool. 

We’ve made progress and covered new ground, granted we can now read the signals but can’t actually interpret them, much like listening to someone speak Latin when you don’t, you know they are are saying something but you’ve got no idea what. 

But still, progress. 

---
<!--
****************insert pictures here of successful tests**************** -->
<video 
    src="../images/10.%20Design%20Studio_Pulse%20Project/Successful%20Test%201.mp4"
    controls 
    title="Successful signal test 1"
    style="border-radius: 5px;"> <!-- Adjust the radius value as needed -->
</video>

<video 
    src="../images/10.%20Design%20Studio_Pulse%20Project/Successful%20Test%202.mp4"
    controls 
    title="Successful signal test 2"
    style="border-radius: 5px;"> <!-- Adjust the radius value as needed -->
</video>

<figcaption> Our first Successful Tests!</figcaption>

---

### So What?

At this point reading through this article ***(and it is a long article)*** you might be thinking, well this is cool and all that but what’s the point?  

> **Why bother trying to read and interpret these signals at all?**
> 

Now that’s a fair question, and one I asked myself many times throughout the project so far. 

Really the point is further try and understand the nature that surrounds us and be able to better interpret the needs of the ecologies that we live in so that we can begin to provide for them in different much more niche ways that we maybe haven’t had the chance to do before. The better we can understand and take care of the ecosystems we are part of, the better they will take care of us. 

How often have you looked at a plant or a tree and thought right, well all it needs is a little soil, some water and sunlight and it’ll be fine, I’m definitely guilty of that. the reality of the situation is that these plants are far more sensitive to their surroundings than we give them credit for, and if we can tap into that sensitivity with modern technology in a non invasive way maybe we can get to the point where we could listen to an entire forest, being able to identify problem areas much much quicker, or be able to listen to and see how the first reacts to the presence of others in it’s midst. That’s what struck me really when I began this project, and the potential for others to carry this on after us to create concepts and ideas that redefine our relationship with the natural world is just so exciting! 

Granted, we actually need to move on and be able to interpret what the signals mean, but that’s what designing with others and in an open source way is all about, that we can share this information with the world and others will build off our research to create something even better. That for me is the most important bit of work so far. 

I’m happy I got to try and do some more technical understanding on this project so far, I think definitely moving forward I want to have a bit more focus on the technical application work, as that was left mostly up to Marius and Nicolo as they had the most Arduino coding experience.  

I think it would be really interesting to develop a way for me to include some of my design skills further in this project, and I’m happy it took the route it did, one of the key themes in my design interests is the theme of solar punk, which is all about using technology and nature in symbiosis to benefit everyone human and non human alike. 

And this project has helped me take one step closer to that future. 

---

---
<!--
****************insert pictures here of timeplanning**************** -->
<img src="../images/10. Design Studio_Pulse Project/Miro Timeplanning.png" alt="Miro Timeplanning" style="border-radius: 5px;">
<img src="../images/10. Design Studio_Pulse Project/non human intelligence & Technology - Ideas.jpg" alt="Future Direction Ideas" style="border-radius: 5px;">

<figcaption> The direction we want to take the project in in the future </figcaption>

---

### What now?

Now we’ve come to the next phase of the project, we’ve discussed what we want to do for it as we head towards the end of the term and the Design Dialogues presentation, and we have a few ideas. 

We want to continue our research into non human intelligence, and we think we might be able to use different stimuli to measure different responses in the plant. Effectively we are trying to create a basic sign interpretation chart, this spike equals sunlight, this one is CO2, this trough is water etc and so on.  Because if we can at least translate what these signals mean then others can begin to develop other solutions from those discoveries. 

> **We are pretty sure we are creating at least a portion of new knowledge with this approach**
> 

We are pretty sure we are creating at least a portion of new knowledge with this approach, so we’ve taken on the task of creating some detailed documentation for the entire project and we’ve planned a series of YouTube tutorials explaining how to build your own circuit board using Arduino so you can read the signals in your own plants yourself at home.

Sharing what we’ve learned in an open source way is how we want to build this project further, we want to engage the community and involve them with us along our design and research journey.  

---
<!--
****************insert pictures here of using working on roof at Iaac?**************** -->

<img src="../images/10. Design Studio_Pulse Project/All of us working on roof.jpg" alt="ALl of us working together" style="border-radius: 5px;">
<figcaption> Continuing our work towards Design Dialogues </figcaption>
---

Personally, I’d like to see if it’s possible to design and build a custom handheld device that you’d be able to put together yourself, which would function almost like a tricorder from star trek, letting you take it out and about with you in a park or a forest, attach it to any plant you find (safely without harming of course) and try and interpret how the plant is communicating. 

That would be something that I think could be really fun to develop and share with the world in an open source way, and showcase some fun and interesting research that I’ve worked on in a tangible and interactive way.

I think if more people could experience that excitement we felt when we managed to first read those signals, that could create some pretty hefty changes in the way we perceive plants!

> **Imagine going on a walk through a forest knowing that the plant life around you is actually reacting to your presence as you walk through it!**
> 

For now, we are preparing this project for design dialogues, we are going to try and create some form of interactive stand we think, where we encourage people to interact with a few plants and see how the signals change within them as they do, visualising it all through something like touch designer. 

I think now it might be too early to think about what we could have done differently, as this project has only just begun really,  and we wouldn’t have got to where we are now if we hadn’t struggled so much with the ECGs in the beginning, but that’s what this stuff is all about, *f***ing about and finding stuff out!*

I’m not sure where this project will lead, if it will lead to some new and exciting product or service, or a more introspective and thoughtful approach to nature. Maybe both, who knows? 

Whatever it will be, it’s exciting times ahead.

---

**you can check out videos of our work so far below 👇**

**Pulse Project Introduction**
<iframe width="560" height="315" src="https://www.youtube.com/embed/v7DfLnNG7B8?si=SqEvxDtTdQsokYEr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

**Pulse Circuit Assembly Tutorial**
<iframe width="560" height="315" src="https://www.youtube.com/embed/3a1IpfX1REI?si=0-JZSsmDnJqWUtdF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
---

# Some Resources:

**Connecting two plats as inputs and outputs:**

https://youtu.be/pvBlSFVmoaw?feature=shared

**Mushrooms “talking” with a MIDI**

https://www.youtube.com/watch?v=c5ULfimE7vA

**Book: Towards Fungal Computing**

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6227805/

**Reading spike signals in plants**

https://backyardbrains.com/experiments/

**Music with plants and ardunio**

https://youtu.be/yuJhKUunYPE?feature=shared

**Musical Mushrooms**

https://youtu.be/J-nIBA0V_No?feature=shared

**Mining logical circuits with mushrooms**

https://www.nature.com/articles/s41598-022-20080-3