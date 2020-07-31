# Marcov-in-Chains

This was a fun little project! As some background, I enjoy noodling on FiveThirtyEight's weekly puzzle problem, [The Riddler](https://fivethirtyeight.com/tag/the-riddler/). The puzzle for the week of May 27th 2020 was as follows: 

> You start with a fair 6-sided die and roll it six times, recording the results of each roll. You then write these numbers on the six faces of another, unlabeled fair die. For example, if your six rolls were 3, 5, 3, 6, 1 and 2, then your second die wouldn’t have a 4 on it; instead, it would have two 3s.

>Next, you roll this second die six times. You take those six numbers and write them on the faces of yet another fair die, and you continue this process of generating a new die from the previous one.

>Eventually, you’ll have a die with the same number on all six faces. What is the average number of rolls it will take to reach this state?

>Extra credit: Instead of a standard 6-sided die, suppose you have an N-sided die, whose sides are numbered from 1 to N. What is the average number of rolls it would take until all N sides show the same number?

My first instinct was to run a simulation program I wrote, serveral thousand times. This got me the result of 9.64 turns (as it turns out I wasn't alone in this). However there is a better closed form solution that I didn't think about using Marcov chains and transition matrices (This returns a result of 9.656 turns).

This got me really interested and I ended up obsessing over the applications as they are really cool! Beyond solutions to fun math riddles, Markov chains have plenty of real world applications randing from use in sampling and bootstrap simulations, to simple predictive text algorithms such as the next word recomendation system in your phones messaging app.

## The project

This is a generative text program I built using R and Julia. I chose to use R becuase I am very familiar with R but was running up against speed constraints while generating bi-grams and sample pools from large corpora. Normally I would pull out some C++ but I have always wanted to use julia and this seemed like a good application. As an example enjoy this text I generated using the program from Alice in Wonderland  by Lewis Carol:

>
