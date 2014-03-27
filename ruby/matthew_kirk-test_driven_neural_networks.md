# Test Driven Neural Networks

Matthew Kirk, Modulus 7, @mjkirk

Writing thoughtfulml.com

* What are feed forward neural networks
* How to classify strings to languages using neural nets
* TDD it

## Neural nets

* Supervised learning
* "The sledgehammer of functional relationships."
* Three layers
    * Input layer - just the inputs
    * Hidden layer - adding complexity to the function, can't see what's going on, like a private method
    * Output later - just the output
* Neurons
    * Neurons are based on threshold logic. Like a digital logic gate or boolean logic.
    * Fuzzy logic works in here somehow
* Activation function - takes any input and makes it between zero and one
    * Learning curve (sigmoid, elliott functions)
    * Bell curve (Gaussian)
    * Line (linear)
    * Periodic (sine and cosine)
    * Threshold (logic)
* Training algos
    * Quickprop
    * RProp
    * Another I missed

## Practicum

* Data collection
    * Used the bible (most translated book in the world) as corpus.
    * Stems, words, counts, letter frequency - he uses letter frequency
* Building the neural net using TDD
    * Test the seams
        * `it hase the proper keys for each sentence`
        * `it sums all character frequences to 1 for each sentence`
        * `it returns characters that is a unique set of...`
    * Test for underfitting
        * `it trains and cross-validates with an error of 5% for each language`
    * Test for overfitting
        * `... ? ...`

https://github.com/hexgnu/language-predictor

