# Usage 
To use our code run root in this directory. When running it the first time it 
will automatically compile the different scripts. For a sample usage see the 
code in `projectDemo.cpp`. To call the `projectDemo` function in `projectDemo.cpp` call 
`projectDemo()` in the root terminal.

To run our different methods first make a `tempTrender` object: 
```
tempTrender city("../data_clean/Lund.csv")
```
Then call our methods on it, for example
```
city.tempPerDay()
```

## Methods Implimented
 * tempPerDay
   * Takes no Inputs.
   * Shows a plot with the mean temperature and the spread for each day of the year.
 * tempOnDay
   * Takes as input the day of the year as an integer,
   * Alternatively pass two integers Month and Day.
   * Plots the spread of the temperature of that day throughout the years.
 * covariance
   * Takes as input another city datafile or another `tempTrender` object.
   * Alternatively pass another city datafile and a minutelag.
   * Ideas for minutelags would be: a day (60*24), a week (60*24*7) or six months (60*24*30*6)
   * Plots the correlation between the two cities.

# Directory structure
The base directory here contains our example code file (`projectDemo.cpp`) which
exemplifies the different methods that we implimented for our project.
It also contains the `rootlogon.C` file which manages the automatic compiling
and linking of our code.

The include directory contains the header files for our code while the `src` 
directory contains the corresponding logic.


