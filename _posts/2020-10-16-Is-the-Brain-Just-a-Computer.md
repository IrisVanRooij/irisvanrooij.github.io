---
layout: post
title: Is the brain (just) a computer?
category: theory, brain, cognition, computing, explanation
---
![brain computer](/images/braincomputer.jpg "braincomputer")

Two weeks ago, I attended the Learning Salon, hosted by [Joshua Vogelstein](https://twitter.com/neuro_data), [Ida Momennejad](https://twitter.com/criticalneuro) and [John Krakauer](https://twitter.com/blamlab), for the first time. Marcin Mi&#322;kowski was speaking on the question "[Why think that the brain is not a computer](https://philpapers.org/rec/MIKWTT)?". Given this topic, obviously I could not resist and signed into the [crowdcast](https://www.crowdcast.io/e/learningsalon/5). I even had opportunity to participate in the discussion "on stage" and shared some thoughts on the question posed. This blogpost is to spell out my thoughts a bit more.



Whenever the question 'Is the brain a computer?' comes up (and [on Twitter it comes up more often than some of us like](https://twitter.com/IrisVanRooij/status/1026498652892790785?s=20)), I have mixed feelings. I agree with Mi&#322;kowski and many of my colleague computational cognitive (neuro)scientists that the usual objections are against a straw man position. I will not repeat those arguments here and will instead just assume that the standard objections have been satisfactorily dealt with by Mi&#322;kowski and others (e.g., see also this great [blog](https://medium.com/the-spike/yes-the-brain-is-a-computer-11f630cad736) by Blake Richards and I've said a few words on these objections in the context of the [tractable cognition thesis](https://onlinelibrary.wiley.com/doi/pdf/10.1080/03640210801897856) myself).

So why am I still uncomfortable?

My discomfort comes from the formulation:

(1) 'Is the brain a computer?'

I have some doubts about the usefulness of this phrasing. In my opinion, the more scientifically relevant and interesting question is:

(2) 'Can we explain (human) cognitive capacities computationally?'

Questions (1) and (2) are not equivalent. But in discussions about (1) they often are treated as if they are equivalent.

Confusion may arise because the words 'brain' and 'mind' are often used interchangeably. I don't think mind and brain are the same thing. I think it is important to keep them conceptually and linguistically distinct. Not because I am a dualist. No worries! I do think mind (or rather, cognition) is physically realized. But I am what one may call an *implementationalist functionalist*; that is, I think that the relation between mind and brain is one of implementation and I do not rule out that "stuff other than brains" could functionally reproduce cognitive capacities that in humans are implemented, in part,  by our brains. I say 'in part', because I am also what one may call an *embodied embedded computationalist* (I know, an oxymoron for many!), which means that I think that [the brain is but one player in an orchestra](https://journals.sagepub.com/doi/10.1177/0959354308089787) that implements cognition. The body and our environment are other key players and are co-constitutive of the 'stuff' that implements our cognitive capacities.

So where does this leave us on questions (1) and (2)?

Let's have some definitions and hope to clear things up.

## Definitions

To **compute** a function $$ f: I \rightarrow O $$ is to transform an initial state (input $$ i \in I$$) into a final state (output $$ o = f(i) \in O$$) in a way that can be described by an algorithm. Here, by **algorithm** we mean a step-by-step procedure with a finite description. According to the [Church-Turing thesis](https://en.wikipedia.org/wiki/Church–Turing_thesis) the notion of algorithm can be formalized by a [Turing machine](https://en.wikipedia.org/wiki/Turing_machine). Indeed, so far, all acceptable formalisations turn out to be equivalent to the Turing machine formalisation, including neural networks, cellular automata or quantum computers [[^1]].

It will be useful to distinguish between different types of algorithms (or "algorithms"). A **deterministic algorithm** is an algorithm with the property that if one reruns the algorithm on exactly the same input it will perform exactly the same steps and, hence, produce the same output. In contrast, a **probabilistic algorithm** is an algorithm that proceeds probabilistically for at least some steps, choosing how to proceed by sampling from a set of options. If one runs such a probabilistic algorithm on the same input many times it will produce a particular distribution of outputs, some more frequently produced than others. A **non-deterministic "algorithm"** (not really an algorithm!) is a fictive or imaginary "algorithm" that at each choice point on how to proceed magically makes the 'correct' next step (or equivalently, makes *all possible* steps in parallel at the same time and then at the end chooses the 'correct' output from the exhaustively generated set). For instance, an algorithm that would "compute" the winning lottery number for any given day, by magically guessing each of the 10 digits of the winning number for that day, would be an example of a non-deterministic "algorithm". I hope it is self-evident that such a magical machine does not really *compute* a function as we understand that term. No deterministic algorithm would be able to compute 'winning lottery numbers' from say 'dates that the lottery takes place' [[^2]], and neither could a probabilistic algorithm compute it with anything but negligible probability ($$p = 0.0000000001$$; no better than rolling ten 10-sided dice). The [probability of being struck by lightning](https://www.floridamuseum.ufl.edu/shark-attacks/odds/compare-risk/death/) is substantially higher.

Lastly, we'll say a function is **computable** if and only if there exists an algorithm that can compute it. We can also safely allow for a notion of **[probablistic computability](https://irisvanrooijcogsci.com/2020/01/01/sampling-cannot-make-hard-work-light/)**, if we can set some non-trivial lower bound on the probability that the returned output is 'correct' (whatever that means).

## Is Cognition Computable?

It is an important question for cognitive science whether or not all cognitive capacities can be explained as a form of computing. According to computationalism (broadly construed [[^3]]) this should indeed be possible. Ultimately it is an empirical question, though. So far, cognitive science has been making good progress in formulating computational models of various cognitive capacities spanning domains such as perception, learning, problem solving, decision-making, language and more. It is also known, however, that such models still have problems scaling beyond toy domains while maintaining a good 'fit' to human-level performance and without running into the problem of [intractability](https://cognitionandintractability.com). This is not proof that computationalism is bound to fail, but it does mean we---computationalists---still have quite a lot of work to do before we have convinced those skeptical of computationalism [[^4]].

## Can Brains Only Compute?

On the one hand, it is obvious that the brain is a computer. Using my brain I can, for instance, do addition --- i.e., compute the sum of two numbers ($$ f: \mathbb{N} \times \mathbb{N}  \rightarrow \mathbb{N} $$, such that $$f(x,y) = x + y$$). I could also use pen and paper to do it, but if the sum is not too complicated I can do it 'in my head'. If a thing $$X$$ having at least one computational capacity is sufficient to call $$X$$ a computer, then by all means, the brain is a computer. Clearly, this is not what all the fuss is about when people ask question (1) 'Is the brain a computer?'. I think most of the fuss is actually about question (2), but as explained above that is an open *empirical* question.

A last possible reading of question (1) is that one may mean to ask 'Is everything that the brain does computing?' I think to that the answer is 'No'. A brain could accidentally guess the digits of the winning lottery number, just as one could guess them by rolling dice or flipping coins, but only by magic or sheer accident would a brain (or any computing machine) guess them correctly. We would not call that computing [[^5]]. What this does mean is that the brain can do things that do not constitute 'computing'. Not because the brain has super-Turing "computing" powers, but just because not all of its behaviours are governed by it computing a function. A corollary is that the brain's behaviour is not exhaustively described by the union set of all its cognitive capacities, and hence even if all cognitive capacities turn out to be computable, the brain would not *just* be a computer.

-- [Iris van Rooij](https://metatheorist.com/about/)

[^1]: At this point I ask the reader not to raise any of the usual objections (e.g., 'but a brain may compute in a way that cannot be formalized by a Turing machine' or 'the brain need not compute over symbols' or whatever just comes to mind). None of these objections are relevant, and in any case, have been dealt with satisfactorily by others (see second paragraph of this blog.)

[^2]: While writing this I realize that what I wrote must be false, since it is known that the set of functions that are computable by a deterministic machine is the same as the set of functions that are "computable" by non-deterministic algorithms. As I want to have this blog out before the next Learning Salon, I will leave it to the reader to find my reasoning error (I have a suspicion; and am happy to discuss to what extent the mistake is damaging for my overall argument).

[^3]: Computationalism here is divorced from representationalism. Both representational and [non-representational](https://link.springer.com/article/10.1007%2Fs11098-005-5385-4) versions of computationalism are possible.

[^4]: Interesting personal detail: I used to be fervent anti-computationalist myself. This was during my Masters' studies in the 90s. At the time, I could not for the life of me imagine how anyone could take computationalism seriously. What changed my mind, during my PhD thesis research, is perhaps the topic for a different blog.

[^5]: Fascinatingly, some people think [they can do better than chance](https://www.wikihow.com/Choose-Lottery-Numbers).

<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>
