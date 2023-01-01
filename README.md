Many real-world scenarios can be characterized as sequences of events, i.e. transitions between states, where the probability of the scenario being in any state is solely dependent on the previous state. This condition of the probability of transitioning to a state depending only on the prior state is what defines a Markov Chain, or Markov Process. For example, say the weather on a given day can be either sunny or rainy. Then, the probability of tomorrow’s weather is only dependent on the the weather today, and the weather on all previous days has no influence. Here, the weather can be modeled as a Markov Chain.

Building on the idea of a Markov Chain is a Hidden Markov Model (HMM). The ’backbone’ of an HMM is just a regular Markov Chain. However in this case, the states are unobservable, or hidden. Each of these hidden states have some influence on the states that are observable, sometimes called signals or symbols. Hence, there are transition probabilities between the hidden states, as well as ”emission” probabilities; the probabilities of an observation occurring given the current hidden state.

In this paper, we aim to:
1. Give an overview of HMMs, introduce basic notation and main problems studied using HMMs.
2. Give various examples to illustrate the theory of HMMs.
3. Use HMMs to study various problems in applications such as political science/voting systems, financial time series, and effect of mental state on video game performance.

We also provide R code that provides tools to compute the forward algorithm, the Viterbi algorithm, and code to create all figures provided in the examples.
