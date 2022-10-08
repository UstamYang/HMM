# HMM
Course project of Hidden Markov Model spellchecke

In this exercise we will make a spell-checker using a HMM. To
do this, download alice nlp release.ipynb and follow the instructions.<br />
 Read through the first two blocks to get an idea of what the task is. The idea is to go through the corrupted
corpus, identify words which have probably been corrupted, and correct them probabilistically.<br />
 In the 4th box, fill in the functions to construct the word probabilities (weighted frequencies in uncorrupted
corpus) and transition matrix (which gives Pr(word | prev word)). <br />If done correctly, the lines printed out
should read<br />
prob. of "alice" 0.014548615047424706<br />
prob. of "queen" 0.002569625514869818<br />
prob. of "chapter" 0.0009069266523069947<br />
with smoothing<br />
prob. of "the alice" 0.00025406504065040653<br />
prob. of "the queen" 0.016514227642276422<br />
prob. of "the chapter" 0.012957317073170731<br />
no smoothing<br />
prob. of "the alice" 0.0<br />
prob. of "the queen" 0.03968253968253968<br />
prob. of "the chapter" 0.0<br />
prob. of "the hatter" 0.031135531135531136<br />
 In the 5th box, fill in the function for computing the emission probability. The first 10 words closest to Alice
should be<br />
[’abide’, ’alice’, ’above’, ’voice’, ’alive’, ’twice’, ’thick’, ’dance’, ’stick’, ’prize’]<br />
 Construct and run your Hidden Markov Model spell checker using the functions computed for the prior<br />
probabilities, emission probabilities, and transition probabilities. List some words whose spelling was corrected<br />
correctly, and some examples where the spell-correcter did not work as expected. Report the recovery rate of
the “fixed” corpu<br />
