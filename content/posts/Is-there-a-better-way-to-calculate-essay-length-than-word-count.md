---
title: Is word count really accurate?
date: 2021-11-10
draft: false
---

Recently, I’ve asked myself this question: _Is there a better way to calculate essay length than word count?_ Just wonderin’. While word count might work fine for a single-page documents, word count becomes less accurate for hundred-page documents, like, um, a PhD thesis.

## The problem

So, here’s the thing. In linguistics, [agglutinative languages](https://en.wikipedia.org/wiki/Agglutinative_language) exist. In other words:

<blockquote>(of a language, e.g. Hungarian, Turkish, Korean, and Swahili) tending to express concepts in complex words consisting of many elements, rather than by inflection or by using isolated elements.
</blockquote>

<figcaption>—Oxford English Dictionary</figcaption>

What this basically means is that some languages have _longer_ words, while others have _shorter_ words. A good example would be Turkish. Like the below image:

{{< figure src="https://qph.fs.quoracdn.net/main-qimg-9d5c124746722c4caaa1a2d06c13a362-lq" title="Comparison of an agglutinative language with a non-agglutinative language" caption="By a deleted account from [Reddit](https://www.reddit.com/r/languagelearning/comments/2hd4em/an_example_of_turkish_languages_agglutination/)." alt="Comparison of an agglutinative language with a non-agglutinative language" >}}

Therefore, a single word in Turkish could make for an entire sentence in English, which is kinda inaccurate if we were to judge document length just by word count. Yes, in technical terms, word count _does_ equal to the byte size of a digital document, but from the aspect of “how much is this person really saying”, word count scores poorly.

## Existing solutions

An interesting point of research is linguist Joseph Greenberg’s work in measuring the “agglutinativeness” of a language. In his [academic paper](https://www.jstor.org/stable/1264155?read-now=1&refreqid=excelsior%3A5f06e207ebd245aaf83c24e72c55976c), the degree of agglutinativeness is based on a ratio: The number of agglutinative junctures to the number of morph junctures. It’s a bit over my head, but the evidence is in the table below, extracted from Luschützky (2003):

<table class="wikitable">

<tbody>

<tr>

<td></td>

<th>Agglutination</th>

<th>Synthesis</th>

</tr>

<tr>

<th>Swahili</th>

<td>0.67</td>

<td>2.56</td>

</tr>

<tr>

<th>Turkish</th>

<td>0.60</td>

<td>2.33</td>

</tr>

<tr>

<th>Yakut</th>

<td>0.51</td>

<td>2.17</td>

</tr>

<tr>

<th>English</th>

<td>0.30</td>

<td>1.67</td>

</tr>

</tbody>

</table>

Solely from the agglutination index, there is a difference 0.37 between the agglutinative Swahili and the non-agglutinative English. So, what does that mean? I suppose it works like this: A text written in Swahili can fit in almost two times more content than a text written in English. So is word count really accurate? Is it really a universal marker of text length? Let’s not even get into Mandarin, which itself is perhaps one of the most agglutinative languages, which was, for whatever reason, seemingly omitted from the aforementioned study.

## Personal thoughts

Based on the above, how then, do we measure document length more accurately? I have a theory. Based on the assumption that clause-binding words/phrases such as “therefore”, “so”, “hence”, “as a result” indicate a certain degree of logical advancement in content, we could instead count these words/phrases in a text such that a greater number would result in a higher “content length” value.

Maybe, we could go even further. What if we could leverage an unsupervised [machine learning](https://en.wikipedia.org/wiki/Machine_learning) model to understand the “content length”? This is a super interesting idea, and could actually be useful. For the time being, while word count still has its place in school, I hope that more robust systems for measuring content length can be developed in the future.