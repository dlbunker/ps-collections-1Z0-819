## Comparison Overview
You should be understand the differences between equals, compare and mismatch

| Method        | Arrays the Same?     | Arrays are Different?                 |
|---------------|----------------------|---------------------------------------|
|equals         | true - memory address| false                                 |
|Arrays.equals  | true                 | false                                 |
|Arrays.compare | 0                    | negative - smaller, positive - bigger |
|Arrays.mismatch| -1                   | index where arrays begin to differ    |


## Arrays Compare Rules
Comparison is done by Comparators and this table will help with the rules around using compare()

| Array 1             | Array 2               | Result       | Why?                                              |
|---------------------|-----------------------|--------------|---------------------------------------------------|
|int[] {1,2,3}        | int[] {1,2,3}         | 0            | arrays are an exact match                         |
|int[] {1,2,3}        | int[] {1,2}           | > 0, positive| array 1 has more elements                         |
|int[] {1,2}          | int[] {1,2,3}         | < 0, negative| array 1 has less elements                         |
|String[] {"abcdefg"} | String[] {"abcdefg"}  | 0            | arrays are an exact match                         |
|String[] {"abc"}     | String[] {"abcdefg"}  | < 0, negative| array1 is a substring of array 2                  |
|String[] {"abcdefg"} | String[] {"abc"}      | > 0, positive| array2 is a substring of array 1                  |
|String[] {"abcdefg"} | String[] {"ABCDEFG"}  | > 0, positive| Upper case is treated as smaller than lower case  |
|String[] {"ABCDEFG"} | String[] {"abcdefg"}  | < 0, negative| Upper case is treated as smaller than lower case  |
|String[] {"abcdefg"} | String[] {null}       | > 0, positive| null is smaller than any character value          |
|String[] {null}      | String[] {"abcdefg"}  | < 0, negative| null is smaller than any character value          |
|int[] {1,2,3}        | String[] {"abcdefg"}  | compile error| arrays must be the same data type to compare      |
