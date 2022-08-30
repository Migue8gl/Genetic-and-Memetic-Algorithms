# Genetic-and-Memetic-Algorithms
Poblation techniques for the Weight Learning Problem.

- This practice was done in the Metaheuristic (Metaheurísticas) subject at the UGR. It consists in study, understand and execute different poblation based algorithms such as genetic or memetic ones to solve the weight learning problem in three different data sets.

### Data Sets:
  * Parkinsons – data used to distinguish presence or absence
of Parkinson's disease. It consists of 195 examples, 23 attributes and 2 classes.

  * Spectf-heart – contains attributes calculated from images
medical computed tomography. The task is to find out if the
physiology of the heart is correct. Consists of 267 examples, 45 attributes
and 2 classes.

  * Ionosphere – radar data collected at Goose Bay. Its objective is to
classify electrons as "good" and "bad" depending on whether they have
some kind of structure in the ionosphere. It consists of 352 examples, 34
attributes and 2 classes.

### Algorithms: (Solutions before known as weights vector are know called chromosomes)
	- AGG: In generational genetic algorithms we start from a
initial population from which a few individuals (selected by binary tournament and with a probability) are crossed with each other. Of each crossing made
two children are obtained. The children, together with the uncrossed parents, are
randomly selected under a probability to be mutated. A
Mutation is a random change (for better or worse) in the genes of
selected chromosomes. Once all this is done, with elitism we choose the
best candidate of the current population, which is introduced in the following
population replacing the worst of the next generation.

    	- AGE: The main difference with the generational variant is that this algorithm cross two parents once each generation. Only two parents will be crossed and under a certain probability their son will be mutated. If the children are better than the worse individuals in the current generation, they replace them. There is no elitism.
    
   	- AM: Memetic algorithms are a combination between genetic algorithms and local search. There will be 3 variations for each genetic algorithm:
      * 1) local search applied to all the poblation.
      * 2) local search applied to certain indiviuals with a probability of 0.1%.
      * 3) local search applied to the best indiviuals with a probability of 0.1%.

-----HOW TO RUN IT-----

1 - To compile run "make" in the terminal.

2 - To run the program go to the terminal and run "./bin/p2 <seed> <parameter>" where
<seed> is the seed we choose and
<parameter> can be:
		-> 1: spectf-heart
		-> 2: parkinsons
		-> 3: ionosphere

--- Other things will get an error ---

[USE] -> A script is attached for a more comfortable execution of the results in text files, the script is "script_acp.sh".
All data sets can be executed concurrently (which makes the individual times of each program greater, but it is faster when it comes to obtain results).
If, on the contrary, it is desired, it can be executed sequentially. All of this is specified in the script itself.
