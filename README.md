## Hopfield Network

The Hopfield network is a recurrent network initially proposed by John Hopfield in 1982.  Understanding the Hopfield Net is a good start for understanding Boltzman Machines and other probabilistic graphical models.

The Hopfield Net is composed of fully connected binary units (that is, each unit is bidirectional connected to every other unit). The binary units normally takes states of {-1,+1} as opposed to {0,+1}.  Each pair on units has a connection weight (wi,j) 

h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x

Because every unit in a Hopfield Net is connected to every other unit bidirectionally, the Hopfield Net is an example of *undirected* graphical model.  The undirected model is in contrast to a directed graph, such as a Bayes Net.  There are two restrictions on the connectivity: 1) no unit can be connected with iteselfand 2) all connections are symmetric.  Constraint #2 (all connections are symmetric) gaurantees that the energy function decreases monotnically while following the activiation rules. If the weights were asymmetric, the model would exhibit oscillations and unstable states.  

### Hopfield Net as Autoassociative Memory

The Hopfield Net is of interest as an *autoassociative memory*.  An autoassociative memory can "fill in" incomplete parts of an input.  Autoassociation is shown in the accopanying Jupyter notebook. `Hopfield.ipynb`
