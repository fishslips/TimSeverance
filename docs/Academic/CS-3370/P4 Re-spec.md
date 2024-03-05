### Strategy

This project used to be called analyze. We're just doing a bunch of data stuff in C++ for this project.

Project is divided into parts:

1) Read analyzation parameters (from .ini files)
2) Read the Data (from .dat files)
3) Negate the Data
4) Smooth the Data
5) Analyze the Data (Detect Pulses)

#### Main

Receive configuration file (gage2scope.ini) via argv[1] 
(Lines with # means comment, ie ignore those lines)

Read and Analyze all dat files in the current directory. We're only using 3, but your code should be able to handle any number of dats.

Display error messages for invalid .dat, but continue
Throw runtime errors for invalid .ini files.

#### Analyze (This will probably be a class)

Copy data from the file into a vector. Remember to negate the data that goes into the vector

Store parameters from ini file here (vt, width, pulse_delta, drop_ratio, below_drop_ratio)

| Parameter        | Description                                  |
| ---------------- | -------------------------------------------- |
| drop_ratio       | A number less than 1                         |
| below_drop_ratio | The number of values less than drop_ratio    |
| pulse_delta      | The gap between pulses to look for piggyback |

**Smoothing**
Iterate through your vector and for every point starting from [3] and ending at 4th from the last, swap out the values in each index with a weighted average using the following formula:

(iter[-3] + 2\*iter[-2] + 3\*iter[-1] + 3\*iter[0] + 3\*iter[1] + 2\*iter[2] + iter[3]) / 15

**Pulse Detection**
Here is where you'll use the parameters you read from your .ini file. 

Iterate through your new values again. For every point, check if the rise (y<sub>(i + 2)</sub> - yi) exceeds vt. If it does, then a pulse begins at i. After finding a pulse, move forward starting at y<sub>(i + 2)</sub> until the values start to decrease before looking for a new pulse. To do so, you can probably keep track and determine 

### Notes

