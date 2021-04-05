#### Name: Alton Caylor
#### Date: 29 March 2021
#### What this is: Calculations from the manual work out of the Needleman-Wunsch algorithm.

### Instructions: Local Alignment calculations
For each entry in the matrix in the lab assignment, there is a letter and you are to place your calculations for each letter below. The first calculation for entry (a) is done for you. Please follow this example in your calculations for the rest of the letters.

Scoring table:


|Score or penalty| value |
|----------------|-------|
|gap penalty      |-1     |
|Mismatch penalty | 0     |
|Match score     | 1     |


a)
- Match or Mismatch: A = A is a match
- Left entry calculation: -1 - 1 = -2
- Above entry calculation: -1 -1 = -2
- Diagonal entry calculation: 0 + 1 = 1
- Max score: 1 from the Diagonal


b)
- Match or Mismatch:               A = T is a mismatch
- Left entry calculation:          0 + 0 = 0
- Above entry calculation:         0 - 3 = -3
- Diagonal entry calculation:      0 - 1 = -1
- Max score: 0 from the Left


c)
- Match or Mismatch:               T = A is a mismatch
- Left entry calculation:          0 - 3 = -3
- Above entry calculation:         0 + 0 = 0
- Diagonal entry calculation:      0 - 1 = -1
- Max score: 0 from the Above


d)
- Match or Mismatch:               T = T is a match
- Left entry calculation:          1 - 1 = 0
- Above entry calculation:         1 - 1 = 0
- Diagonal entry calculation:      1 + 1 = 2
- Max score: 2 from the Diagonal


e)
- Match or Mismatch:               G = A is a mismatch
- Left entry calculation:          0 - 4 = -4
- Above entry calculation:         0 - 1 = -1
- Diagonal entry calculation:      0 - 2 = -2
- Max score: -1 from the Above


f)
- Match or Mismatch:               G = T is a mismatch
- Left entry calculation:          0 - 2 = -2
- Above entry calculation:         0 + 1 = 1
- Diagonal entry calculation:      0 + 0 = -1
- Max score: 1 from the Above



(Did you remember to add your name to this Markdown file?)
