## Introduction

You want to send your friend a package with different things. Each thing you put inside the package has such parameters as index number, weight and cost. The package has a weight limit.

Your goal is to determine which things to put into the package so that the total weight is less than or equal to the package limit and the total cost is as large as possible.

You would prefer to send a package which weights less in case there is more than one package with the same price.

### Input

```
81 : (1,53.38,€45) (2,88.62,€98) (3,78.48,€3) (4,72.30,€76) (5,30.18,€9) (6,46.34,€48)
8 : (1,15.3,€34)
75 : (1,85.31,€29) (2,14.55,€74) (3,3.98,€16) (4,26.24,€55) (5,63.69,€52) (6,76.25,€75) (7,60.02,€74) (8,93.18,€35) (9,89.95,€78)
56 : (1,90.72,€13) (2,33.80,€40) (3,43.15,€10) (4,37.97,€16) (5,46.81,€36) (6,48.77,€79) (7,81.80,€45) (8,19.36,€79) (9,6.76,€64)
```

### Output

```
4
- 
2,7 
8,9
```

### Prerequisites

To compile and run the project, the following tools should be installed:
* JDK 8+
* Junit
* Maven

###  Classes Uses in Program
com.mercateo.assignment.Application is the main class which invokes com.mercateo.assignment.packer.Packer

Packer class takes help of the following classes to do the work

com.mercateo.assignment.parser.FileParser to convert file text into com.mercateo.assignment.model.Package

com.mercateo.assignment.validator.PackageValidator to validate the data

com.mercateo.assignment.solution.KnapsackSolver to solve the problem

com.mercateo.assignment.presenter.ItemPresenterStrategy to print the solution


### Clone this repository
```
https://github.com/faridhaq1403/package_challenge.git   
```

### Installing

To install type:

```
mvn install
```

### How to run

```
mvn spring-boot:run -Dspring-boot.run.arguments="{filePath}"
```


### Executing Test
 ```
 mvn clean test
```