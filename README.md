# DotNetClasses

In this repository i am trying to add c# example which can be useful to others.

# LINQ

# Aggregate fun
       // using aggregate function . aggregate extension method used to group moltiple row in single group
       // example to combine string array with linq
       string[] sArr = { "India", "USA", "UK" }; 
       string sCountries = sArr.Aggregate((a, b) => a + ',' + b);
       
       //multiplying array with lambda exp
        int[] arr = { 1, 2, 3, 4, 5, 6 };
        int mul = arr.Aggregate((a, b) => a * b);

        // mul with seed value. seed is constant value
        mul = arr.Aggregate(10,(a, b) => a * b);

        // how aggregate function work
        // by specifying parameter (a,b) each no is taken from array in var a, b and multiplied 
        // and put back in a var. it goes untill last index found.
