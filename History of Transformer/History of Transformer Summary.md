# Early computer

The history of modern computer can be traced back to the 1930s and 1940s, when
researches and engineers worked to develop an electronic digital machine that performs
mathematical computation and logical operations. In 1950, Alan Turning introduced his
famous Turing test, which was used to justify if a machine, or a computer, possesses
intelligence. This has inspired the later research and development of artificial intelligence
and a questions here is that can a computer behave like a real brain.

# Biological connection

In a biological system, such as the human brain, neurons communicate via action potentials
and synaptic connections. The human brain contains billions of neurons and trillions of
inter-neuron connections, based on which a neural network forms and it supports our
perception and thinking. Learning on the other hand, is governed by synaptic plasticity, as in
Hebb’s theory: Neurons that fires together wires together. Biological system has inspired the
development of artificial neural network. Similar to the brain, a computational neural
network consists of artificial neuron units, layers, with extensive and complicated
inter-connections. The system can encode and process information through activities of
artificial neurons and the adjustment of inter-neuron connectivity.

In the early 1900s, Lapicque modelled neural activities as electrical circuits, and in the 1950s,
Hodgkin and Huxley developed a more biologically plausible mathematical neural model (the
Hodgkin and Huxley model) that operates based on simulated neuron ion channels. In 1957,
an algorithm called the perceptron was implemented for learning and classification of
images, mimicking tasks that our brain would be able to do.

# Convolutional neural network

Boosted by the further development of computer science and technology, which allowed for
more computational power, more complicated neural network models have been
constructed. A typical example is the recurrent neural network, introduced by John Hopfield
in 1982. It contracts a uni-directional neural network by having bidirectional (or recurrent)
connections between neuron layers. This arrangements allows the output of some neuron
nodes to affect their subsequent inputs, enabling “memory” of information from the past.
This property makes recurrent neural network adaptive to the processing of sequential
information, such as predicting the next word of a sentence based on existing contexts. The
network has been used in areas such as visual simulation and image coding.

# Long short-term memory

Long short-term memory is a variance of the recurrent neural network, introduced in 1997
by Hochreiter and Schmidhuber to address the vanishing gradient problem of the
conventional recurrent neural network. The problem could happen in a recurrent neural
network models with a large number of layers. Learning is characterised as the gradient of
change in neural connectivity in a neural network, and it is driven by back propagation.
Through back propagation, gradient is computed by taking derivative layer by layer from the
late most layer to the very initial layer. If the number of neural layer in a network is large,
the gradient, or the amount of synaptic weight change can be come diminishingly small for
the initial layer these repetitive derivative operations. Long short-term memory uses what is
called “cell state” to carry information from earlier times steps to later time steps and
preserve the long term dependencies in a data sequence.

# Transformer

Transformer is a type of neural network specialized for sequence data processing, similar to
recurrent network and long short-term memory. Though it has several advantages.
Transformer utilizes an “attention” mechanism, which allows the focus onto different
different part of an information sequence. And this mimics the way how human would pay
attention to different parts of a sentence and extract the relation between different words
and the overall meaning of the sentence. Several attention mechanisms can be run in
parallel to attend to different parts of a sequence, called ”multi-head attention”. In general,
transformer possesses good parallelizability and scalability, enabling it to be used on large
datasets and complicated language processing tasks.

# Transformer structure

The transformer model has two components. The encoder takes in the data sequence, in the
form of embeddings. In nature language processing, an embedding is typically the
representation of the meaning of a word, in the form of a vector. The decoder on the other
hand, generates an output sequence. Both the encoder and the decoder contains multi-head
attention mechanisms and a feedforward neural network.

# Attention mechanism

The attention mechanism involves the computation of attention score. Attention score
measures the strength of relation between a word in a sentence with all other words, and it
relates to three key element: query, key and value. In a nature language processing context,
the query can be regarded as a question. The key is a set of contexts that are potentially
relevant to the query. The value is the target, or the answer to be searched for given the
query and the key.

# Attention computation

The attention score is calculated by multiplying the query with the key. A softmax function is
then applied to the product to calculate the weight to be assigned to each key-value pair. It
will then be multiplied with the values. And the output of the attention mechanism can be
regarded as a weighted sum of the values.

