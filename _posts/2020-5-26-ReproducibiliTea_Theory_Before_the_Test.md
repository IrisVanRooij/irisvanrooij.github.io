---
layout: post
title: "Can you give an example of a good theory?"
category: theory, metatheory
---


Last week, I had the pleasure of attending a paper discussion of "[Theory before the test](https://psyarxiv.com/7qbpr)". Eirini Zormpa and Johannes Algermissen organized the discussion for ReproducibiliTea Nijmegen, an [OSCN](https://openscience-nijmegen.nl) initiative.


<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

Many questions and issues were raised. Time flew by. So only some questions could be discussed in depth. Below, I've compiled a list of (paraphrased) questions with a more extended answer.

**1. Does a computational-level theory merely specify the inputs and outputs?**

>The short answer is No. The longer answer: A (formal) computational-level theory is a well-defined [mathematical function](https://en.wikipedia.org/wiki/Function_%28mathematics%29) or [computational problem](https://en.wikipedia.org/wiki/Computational_problem). For instance, to define the capacity for "multiplication" it doesn't suffice to say that this capacity maps numbers to numbers (even though that is true). To distinguish it from any other function mapping numbers to numbers (e.g. addition, square root, a random mapping, etc.) one needs to specify that it maps numbers $$a$$ and $$b$$ to the [product](https://en.wikipedia.org/wiki/Product_%28mathematics%29) of the two numbers, i.e., $$a \times b$$. The same expliciteness is needed for specifying computational-level theories of more interesting cognitive capacities (e.g., how we transforms sensory information into perceptual interpretations or how we transition from beings who cannot speak language to beings that can). But beware! Those functions will of course be much more intricate and difficult to specify than simple arithmetic functions.

**2. Does specifying the input-output mapping require specifying an algorithm?**

> Again, the short answer is No. An 'input-output mapping' is just a different word for 'function'. Specifying a function does not require specifying how the function can be computed. In fact, some functions are [uncomputable](https://en.wikipedia.org/wiki/Computability_theory#Computable_and_uncomputable_sets), i.e., no algorithm exists for computing them [[^1]].  [Computable](https://en.wikipedia.org/wiki/Computable_function) functions, on the other hand, can be computed by different (in principle, infinitely different) algorithms. Take again the example of multiplication. The function $$f(a,b) = a \times b$$ can be computed by, say, the partial products method or by repeated addition (see page 2 of [Theory before the test](https://psyarxiv.com/7qbpr)). Specifying a function is thus not the same as specifying an algorithm.

**3. Why exclude look-up tables? Do they not specify functions?**



><img align="right" width="25%"  src="/images/LookUpTable.pdf">   A look-up table specifies a function by explicitly listing input-output pairs. Consider, for instance, the look-up table on the right that exhaustively specifies a function $$g: X \rightarrow \mathbb{N}$$ mapping inputs in the finite domain $$X = \{(a,b) : a, b \in \{1, $$ $$  2, 3, 4, 5\} \}$$ to the set of natural numbers $$\mathbb{N}$$. In [Theory before the test](https://psyarxiv.com/7qbpr) (fn. 10), we exclude look-up tables as computational-level theories. One may ask: "Why? Do they not specify valid functions?" Yes, they do. But not all functions yield computational-level explanations. Look-up tables lack explanatory value. I suspect you'd agree if you consider applying the idea to your own research.

> Imagine you study a system's capacity and design an experiment to tap into that capacity.  Using two independent variables $$a$$ and $$b$$, each with different 5 levels, you construct 25 conditions. You observe that in condition  $$(a = 1, b = 1)$$ the systems does $$1$$, in condition $$(1,2)$$ it does $$2$$, in condition $$(3,4)$$ it does $$12$$, in condition $$(5,4)$$ it does $$20$$, and so on, exactly as specified by $$g$$. Now, imagine you want to publish $$g$$ as your computational-level explanation of these findings. Do you expect reviewers to be impressed? More likely they will complain you are trying to sell a data table as a "theory". If instead you would postulate that the regularities observed can be explained by the hypothesis that the system is computing $$f(a,b) = a \times b$$ then you not only explain **why** the pattern is as it is, but you also greatly increase the scope (or generalisability) of the theory beyond the domain of your experimental conditions. There is more that can be said about why look-up tables are poor theories [[^2]], but I hope the thought experiment gives enough intuition to move on.

**4. Can you give an example of a good theory?**

> When asked this question during the paper discussion, I was hesitant to give examples. Several thoughts crossed my mind [[^3]], but I realized the question may be motivated by a hope: If one knows what a "good theory" looks like then one may be able to make theories oneself. I am not convinced things work this way. Like one does not learn to paint by looking at paintings, one does not learn to perform experiments by looking at experiments, and one does not learn to develop theories by looking at theories. So I answered: I think it may be more fruitful to ask "how can I learn to do theoretical research?".

> How do we learn new skills? By practice, including trial and error---a lot of error. That said, I can imagine it does help to see examples of how computational-level theories can be **built** from verbal theories (including some trial and error). Check out [Chapter 1](http://metatheorist.com/Chapter-1-freely-available/) of our book for an illustration in the domain of decision-making (more illustrations are under construction). I also think we did a good job of giving some insight into this process in this [paper](http://www.socsci.ru.nl/irisvr/papers/mueller_1_29.pdf) on similarity judgments [[^4]].

**5. I had no training in theory. How can I be expected to develop theories?**

> I think it cannot be reasonably expected. One needs to train in theoretical research in order to do theoretical research, just as one needs to train in experimental research to do experimental research. Unfortunately, historically, psychology curricula have been lacking formal theoretical training. I'd like to bring change to this and am developing some new training tools as we speak. But we can use more of them, of course.

If you have more questions or comments, please send me a message on [twitter](https://twitter.com/IrisVanRooij).

### Footnotes
[^1]: For instance, [Alan Turing](https://www.cs.virginia.edu/~robins/Turing_Paper_1936.pdf) proved that a function that takes as input "an algorithm $$A$$ and an input $$i$$ for $$A$$" and gives as output "true" if and only $$A$$ halts on $$i$$ (and "false" otherwise), is uncomputable.
[^2]: For one, they grow unreasonably large very quickly and for infinite domains they are even impossible
[^3]: I could give some of my own favorites, but reasonable people may disagree that those are genuinely good theories. Also, a lot depends on what is meant by "good". And even if I'd identify a truly good theory, it could be hard for anyone to appreciate *why* it is good, unless one already has substantive knowledge about the content area.
[^4]: This paper is probably an exception. Published papers seldom describe the trial and error process and instead publish the outcomes of the process (plus some experiments to test the proposed theory). Given this tradition it is perhaps unsurprising that theories seem to come out of thin air.  


<a href='https://www.symptoma.es/'>www.symptoma.es</a> <script type='text/javascript' src='https://www.freevisitorcounters.com/auth.php?id=ffbbfa98da26dd5367373b4d525961f859ebeefb'></script>
<script type="text/javascript" src="https://www.freevisitorcounters.com/en/home/counter/746882/t/4"></script>
