---
title: "Natural Language Processing on 'The Stormlight Archive'"
excerpt: "Performed topic modeling and natural language processing on a fictional book series.<br/><img src='/images/NMF_tSNE_ByPage.png'>"
collection: portfolio
---

For my third Metis project, I did topic modeling and natural language processing on a fictional book series by Brandon Sanderson, called "The Stormlight Archive." I first processed the text in chapter and page-level increments using NLTK and standard text pre-processing techniques. I then used various topic modeling techniques, ultimately choosing NMF topic modeling since it performed the best without much tuning. The topic modeling converged naturally on the main characters themselves, and the distribution of pages per character-topic can be seen in the figure below.

<img src="/images/NMF_AllBooks_ByPage.png" height="400"/>

The second figure shows a t-SNE plot of the character-topics, using the NMF topic vectors as input, and shows the level of interaction between characters. This is especially apparent in the middle region, where the NMF topic modeling had a harder time choosing one specific character-topic. After the initial topic modeling, I performed topic modeling of the individual characters in order to determine character-specific thematic topics. Please see the [project GitHub page](https://github.com/nkinnaird/StormlightArchiveNLP) for more extensive details.

<img src="/images/NMF_tSNE_ByPage.png" height="400"/>
