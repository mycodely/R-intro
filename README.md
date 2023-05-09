# R-intro
Resumes, Exercises and newbie courses!

Vectors
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

