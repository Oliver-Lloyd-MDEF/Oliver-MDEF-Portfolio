# The Machine Paradox

We are constantly surrounded by a paradigm of interfaces, old interfaces being replaced by new ones. 
>
*i.e a simple light switch being replaced by a natural language processer like alexa connected to the light bulb itself*
>

As we create more and more complex machines, the interfaces change to become more hidden and obscure, by which I mean we are less able to discern straight away how one input will affect another. The course of the next two weeks is is known as the Machine Paradox, where we will be exploring and understanding just how our much our lives have changed as technology has developed, how machines that once served a vital purpose in our lives have been replaced by newer and different technologies, and figuring out how to hack and modify these old machines to serve a new purpose and bring new meaning to their existence, rather than just let them go to waste. 

## Day 1 (17/10/2023) - Unpacking & Disassembly

In groups, we got together and tear down a product, find out why it failed, how it failed, how it could be repaired, where it was made and create a forensics report to document this entire process. 

In our different groups we went and picked out a broken machine from the fablab deposit on the main floor of the IAAC building.  In our case we chose an old microwave — which was great fun as this is something that most people never think of tearing down as they are such long lasting products, which made it even more interesting to find out why it didn’t work. 

We started to tear down the microwave to get access to it’s insides and began our analysis of the individual parts. Inside we found as expected, a magnetron (the microwave emitter) , a transformer that powered the magnetron and provided it with the high amounts of power it needed, various switches that activated the different functions of the microwave, two motors and a lightbulb. What surprised us (which in hindsight probably shouldn’t have as it’s quite old) was just how simple the insides of the microwave actually was. with most of the connectors being removable clips it showed us that this analogue machine (by which I mean it didn’t have a digital computer acting as a brain behind it) was designed to have multiple components easily replaced as nothing was soldered directly to the board (except components making up the power supply). While it wasn’t exactly easy to access some of the components (like the switches) it was nice to see that this product was indeed designed to be replaced if needed. The only thing that wasn’t fully easily replaceable was the power cable, and only it was because it was directly soldered to the board. 

We started to combine our findings from the teardown into a “forensic report” where we began to detail exactly what we found out about our product, how the different pieces were manufactured, where they were made, how they fit together and just exactly what was wrong with it. 

So far this has been a really great exercise in reframing the way we understand the products we interface with and how we can repurpose and change the technologies around us to truly attempt to give them a second life.

**link photos of labelled exploded view of the microwave on the table, a photo of all of us together with the product, gifs of the tear down, gifs of how different components work**

## Day 2 (18/10/2023)  - Fault testing forensics

Today we began testing each of the microwave components to see what was working and what wasn’t. Most of the microwave components rely on AC power instead of usual DC, with only a few small components requiring DC which made testing components easy and slightly dangerous at the same time as we tested the different AC components using a power cable connected to the mains, which would be soldered or attached with various crocodile clips to the components we were testing. 

Through our testing we discovered that the fault lay with the microwave emitter or the transformer, as every other component would function as intended or turn on when power was supplied — our shouts of joy as the microwave light turned on for the first time as we powered it on were enough to show how much we were enjoying ourselves. 

I was surprised to learn that the entire system of the microwave had been wired in series, which meant that if one component failed (even something as small as the light bulb) the entire system would shut down and stop working. I now know that this was probable done for safety, as you wouldn’t want a microwave magnetron to continue to perform it’s function if the door sensor was broken and couldn’t tell if it was open or closed, but still, this machine was clearly not designed for for easy repairability despite the abundance of spare parts available. 

We continued to finish off the forensics report to document everything we’d discovered so far as well as including our discoveries of what worked and what didn’t as well starting to include the videos and photos of our process, and a map we’d created tracing where each component was manufactured and shipped out across the world. 

As a final part of the day, we ended up jumping and began to control our components individually, turning them on to create their function.

## Activity 3 - Hacking and controlling (19/10/2023)

Today we spent time hacking our way into the various electronic components of our microwave, soldering connectors onto the motors so that we could reconnect them to the original AC power supply the microwave used, and then writing what code we could that would allow us to control the various pieces and the circuit we’d created via an Arduino board. We were trying to give an analogue machine a digital brain. After some trial and error it worked! we are able to sideload some instructions onto our system that would allow the circuit to turn on and off on a 10 second timer. Connected via a relay, we are able to control exactly when and how the motors would turn on, the next task (which I assume is coming later in the week) is to figure out a way to separate both motors from each other, as right now, the induction motor we salvaged (***insert picture below)*** which was originally used to spin the cooling fan splits the high level of voltage coming from the AC power supply into a two separate streams, with the fan motor pulling the majority of the voltage and leaving 30V over to power the motor that originally span the plate inside the microwave. However, while this is really useful inside a microwave, it means that currently the plate motor can only spin when the fan motor is on. So in our quest to create an almost useful machine — in our case we’ve been thinking of turning the microwave into a spinning disco light) we have to deal with a motor that will only work if the other is powered on and running, which might or might not turn out to be useful. Who knows, maybe our disco light will provide cooling air conditioning at the same time…

In any case, this was a really great exercise in getting to know the intricacies of debugging old analogue components, hacking them to work with the digital interfaces we work with now to create something new, debugging again and repeat until finally we can breathe new life into old tech that would otherwise have gone to waste. If anything can teach about how we can design products to better fit into the repairable and circular models of product design and product that we are moving towards it’s definitely this module! I’m excited to see how this project will turn out and what exactly we will create!

Finally we shared our forensic report we’d written about our microwave with the class, explaining how we’d torn down the machine to get into its inner workings, how we tested each component to find out what was wrong with it, how we’d found out what each component was made from and where it came from and what we’d learned from tearing it down and debugging it. This was a really great way for all of us to learn about our various objects and start to build and see connections between these machines and how they can be redesigned for a better more circular future (I think anyway).