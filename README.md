# War-and-Random-Numbers
implements a pseudo-random number generator (PRNG) using the characters from the text file "war-and-peace.txt."
This code demonstrates a simple implementation of a pseudo-random number generator using characters from a text file as the source of randomness. The generated random numbers are then analyzed to compute basic statistics such as minimum, maximum, and mean.


This Python code defines a class WarAndPeacePseudoRandomNumberGenerator which serves as a pseudo-random number generator (PRNG) using the text file "war-and-peace.txt". Here's a breakdown of the code:

Class Definition:

WarAndPeacePseudoRandomNumberGenerator: This class represents the PRNG. It has two methods: __init__ and random.
Constructor (__init__):

Initializes the PRNG object with an optional seed. If a seed is provided, it sets the random seed using the random.seed() function.
random Method:

Generates a pseudo-random number between 0 and 1 using characters from the "war-and-peace.txt" file.
Reads the content of the text file into a string variable text.
Selects a random index within the range of the length of the text and retrieves the character at that index.
Converts the ASCII value of the character to a floating-point number between 0 and 1 by dividing by 255.
Returns the generated pseudo-random number.
Usage:

Creates an instance of WarAndPeacePseudoRandomNumberGenerator.
Generates 10,000 pseudo-random numbers by calling the random method in a list comprehension.
Calculates and prints the minimum, maximum, and mean of the generated random numbers.
