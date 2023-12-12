# Extended Intelligences - Demystifying AI

<aside>
📝 <strong>TL;DR:</strong>
In the Extended Intelligences module, we explored AI development and it’s implications. We visited the CCCB Museum exhibit on the evolution of AI, from Turing to modern systems. Class unveiled the inner workings of neural networks. Using Google CoLab and APIs like Replicate to understand complex models. Crafting "Green Guardian," an AI for plant care, was a rewarding, though initially complex, journey. We're the first AI-immersed generation, but we must consider biases and overreliance on AI. Understanding AI's basics and coding in Python reshaped my view—AI has potential, but ethical development is crucial. The energy consumption and environmental impact of widespread AI models remain a question worth exploring further.

</aside>

---

## Augmenting human experience with machine intelligence

This past week, we dove headfirst into the Extended Intelligences seminar taught by Pau Artigas. Kicking off with a visit to the CCCB Museum, where we explored an exhibition on the development of AI, from its conceptual inception from researchers like Alan Turing to the incredible capabilities of modern generative AI systems. We delved into the implications of AI in our lives, pondering questions like when an AI could be considered "alive" and the ethical dilemmas surrounding AI in weaponry.

In class, we dissected the workings of AI systems and how they are built. Learning how neural networks work, how they are built up of different models, and that an AI system is only born once it has been trained on vast quantities of data after (many) hours of training and retraining on that specific data. 

> A good analogy of a neural network is like a child learning to ride a bike — the child is the program, the data set is the bicycle, and training is like teaching the child to ride.
> 
<img src="../images/09. Extended Intelligences/a_digital_illustration_of_a_small_robot_learning_to_ride_a_bike.png" alt="A Neural net in training" style="border-radius: 5px;">
<figcaption style="text-align: center;">Training a neural network is a lot like teaching a kid to ride a bike</figcaption>

Throughout the seminars, we used google CoLab to run various neural networks from the open source library HuggingFace (filled to the brim with different kinds of neural nets trained on all sorts of data, you can find out more about those [here](https://huggingface.co/)) This was incredibly helpful as (along with a lot of Pau’s guidance) we were able to break down the different programs into their various building blocks and understand how each step worked within the system to create the entire network. We linked these models in the virtual environment from google CoLab through various APIs, as running them locally (especially when training them on the various datasets we wanted to use) would be incredibly resource intensive on most of our machines. These API’s came from various model libraries like [Replicate](https://replicate.com/).

This practical approach, as well as mixing in a good amount of theory to give us the legs we’d need to stand on when exploring this topic (and barely scratching the surface I might add) using tools like Replicate and Google CoLab, made complex AI concepts feel much more accessible.

Learning in this environment was invigorating—I found myself drawn into the discussions and group collaborations. 

### Green Guardian:

We also split into groups to try and create our own models, using various models and training data sets we found online to create a unique AI tool to serve a specific purpose. In our case, we created “Green Guardian” a neural net for plant illness identification and care paired with a generative large language model to provide real-time identification and advice for how to best treat various plant diseases one might come across at home or in a vegetable patch.  Collaborating with Nicolo, Jorge, and Carmen, we found a dataset, worked on image classification neural nets, and connected a generative text AI model called llama to provide care advice—a task that initially seemed really complex but we managed and it ended up being incredibly rewarding, we all were all so genuinely surprised when it worked the first time as none of us had had any real experience with coding python before. 

[For a detailed breakdown of Green Guardian click here](https://drive.google.com/file/d/1qzXcHo4rjvVgh9oJS4lcSBHTrknBFpDq/view?usp=sharing){: .md-button .md-button--primary }

**Find an overview of Green Guardian below:**
<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vQh36qYzr9nni-CzO725eylQa5YG4nYexDU8B1__jbAkOO0YsHOCK_9JlmvFQjK9kxJXqy4qguhHXnR/embed?start=true&loop=true&delayms=5000" frameborder="0" width="1440" height="929" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

**Check out Green Guardian in action here:**
<iframe width="560" height="315" src="https://www.youtube.com/embed/yW7W0c9UYr0?si=vcwCYg3AX9mYdrmj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Final Thoughts

I'm really glad we had this module. I think we're the first generation (*And I don't mean generation in the sense of like a 10 - 15 year gap*), of people that have really sort of embraced AI fully. Ever since the launch of OpenAI's ChatGPT last year. I think that's why we're all so interested in it, because we've all been using these AI tools much more visibly and in some cases (*like mine*) almost daily. 

We've seen what they can do and we've been exposed to how they can create these incredible, incredible things, helping us with so many tasks that before took us much much longer. 

The I think that this entire week has been really interesting because we not only had to learn about developing these AI systems, we learned about how they're built and what they're trained on. But in particular they put a lot of emphasis on the bias that can happen in these models based on the training data and how important it is to have incredibly varied training data to overcome this, but it’s getting that varied training data that can be really difficult, and an AI model is only as good as the data its trained on. 

> An AI model is only as good as the data it’s trained on.
> 

One of the key things that I'm taking away from this module is that this is another transition in our world and we've opened the box. AI is out there, and we're using it all the time, but it feels as though we haven’t given the proper attention and thought as to how these models are actually working: 

- what data sets are they built on?
- Is this reinforcing biases we already have?

> **Or more importantly, is our increasing reliance on these tools to parse and interpret all the information in the world around us beginning to make us overly reliant on them?**
> 

This question even came up when we were building Green Guardian. Would you end up just relying on the AI for diagnosis or would you still go and check somewhere else? I think that there's a real risk that we just become overly reliant on these models, as they make it so easy to offload a lot of the grunt work of thinking.  

At the moment all AI’s (***at least to my knowledge but I would love to learn I’m wrong***) still suffer from machine hallucinations —***this is where they just make stuff up*** — that could lead to some misdiagnoses and completely ruined crops if a more advanced system like Green Guardian was used on a large scale.

The best part of this module was how easy it made to it to understand the basics and some of the nuances of AI research in the quest for machine intelligence.  It gave me a new appreciation for coding, especially coding Python. It always seemed like a scary foreign language, but now I understand it a bit more, I understand it’s utility and it gives you this real window into how these systems work and the language that makes them tick. 

AI is a new, fantastic and amazing tool, it has the potential to do a phenomenal amount of good in the world, pushing us into exciting new futures that benefit everyone, but if we don't put the safeguards in now and understand that if we're going to create and use these models, we need to make sure that the training data we give it is as diverse and different as possible, that whatever data we train them on is fairly compensated to the original creators of that information and that we strive to develop these systems as ethically as possible. 

---

**Finally there’s one last question that’s been playing on my mind since finishing this module, the large language models we’ve gotten so used to using require an incredible amount of energy, not only to train them in the beginning but also to maintain the cooling necessary to keep the servers they operate on happy and healthy.**

**So I’m left wondering, what exactly is the environmental impact of these models that are so widespread now? How much does a ChatGPT prompt cost in CO2 emissions? This an interesting area to explore and something I’m going to try and develop further as the masters program progresses.**
