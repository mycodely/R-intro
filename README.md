# R-intro
Resources to learn data science: Summaries, exercises, and beginner courses based on https://intro-to-ds.netlify.app and https://github.com/paulovillarroel/curso-ciencia-datos

## Vectors
As indicated earlier, a vector has a homogeneous data structure meaning that it can only contain a single type among all the data types. Therefore, when more than one data type is provided, R will coerce the data into a "shared" type. To identify this "shared" type we can use this simple rule:

logical < integer < numeric < character,


We can also use negative indices which are used to remove elements in a vector. Here are some examples:
(x = c(1,2,4,5,1))
```
[1] 1 2 4 5 1                                                //OUTPUT

```

x[-1]
```
[1] 2 4 5 1                                                  //OUTPUT
```

or its last element:
x[-length(x)]
```
[1] 1 2 4 5                                                  //OUTPUT

```

Finally, it is also possible to use boolean value to extract the elements of a vector. This is another useful approach. Here are a few examples:

y = c(1,2,3,4,5,6,7,8,9,10)

y[c(F,T)]

```
[1]  2  4  6  8 10                                           //OUTPUT

```
Recycling is a feature in R that allows operations to be performed on vectors of different lengths. Instead of throwing an error or requiring the vectors to have the same length, R recycles or repeats the values of the shorter vector so that it has the same length as the longer vector. This allows vector operations to be performed more easily.

