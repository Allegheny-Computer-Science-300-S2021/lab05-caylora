#### Name: Alton Caylor
#### Date: 29 March 2021
#### What this is: Questions in blue from the assignment sheet.

#### Part 1.


 1. Which software did you use to conduct your analysis?

http://experiments.mostafa.io/public/needleman-wunsch/

 2. How similar were the two sequences (`s1.fasta` and `s2.fasta`) which you applied an alignment program?

 The two sequences had segments within them that were fairly similar.


 3. Are the two sequences closely related to each other, in your opinion?

 In my opinion, the two sequences are likely related to one another, though perhaps not too closely due to the number of mismatches and gaps.


 4. What proof do you have to suggest such a claim?

 Performing the Needleman-Wunsch algorithm provided a score of 10, which indicates a fairly good match.




#### Part 2
 1. How much similarity exists between each of the sequences to the others?

 Each sequence is fairly closely related to each of the others.


 2. Based on your results so far (which are too few to provide a comprehensive study), do you believe there is evidence that human adaptation is occurring in H5N1 viruses that might merit concern about human-to-human transmission in the near future?

 There are many similarities between the sequences, but the few differences may indicate mutations that could lead to human-to-human transmission. I do not think that the scale of differences indicates a high chance of this mutation occurring, but it is possible.


 3. Statistics: What were the numbers of Lengths, Similarities, Gaps and Scores for each of your alignment tasks?

 AB: 
 ```
 # Length: 1776
 # Identity:    1690/1776 (95.2%)
 # Similarity:  1690/1776 (95.2%)
 # Gaps:          45/1776 ( 2.5%)
 # Score: 8286.0
 ``` 

 AC:
 ```
 # Length: 1751
 # Identity:    1681/1751 (96.0%)
 # Similarity:  1681/1751 (96.0%)
 # Gaps:          20/1751 ( 1.1%)
 # Score: 8205.0
 ```

 BC:
 ```
 # Length: 1776
 # Identity:    1731/1776 (97.5%)
 # Similarity:  1731/1776 (97.5%)
 # Gaps:          25/1776 ( 1.4%)
 # Score: 8575.0
 ```



```AB
########################################
# Program: needle
# Rundate: Mon  5 Apr 2021 18:36:18
# Commandline: needle
#    -auto
#    -stdout
#    -asequence emboss_needle-I20210405-183614-0698-23016510-p2m.aupfile
#    -bsequence emboss_needle-I20210405-183614-0698-23016510-p2m.bupfile
#    -datafile EDNAFULL
#    -gapopen 10.0
#    -gapextend 0.5
#    -endopen 10.0
#    -endextend 0.5
#    -aformat3 pair
#    -snucleotide1
#    -snucleotide2
# Align_format: pair
# Report_file: stdout
########################################

#=======================================
#
# Aligned_sequences: 2
# 1: A_chicken_Viet_Nam_10_2005_(H5N1)_segment_4
# 2: A_China_GD01_2006_(H5N1)_segment_4
# Matrix: EDNAFULL
# Gap_penalty: 10.0
# Extend_penalty: 0.5
#
# Length: 1776
# Identity:    1690/1776 (95.2%)
# Similarity:  1690/1776 (95.2%)
# Gaps:          45/1776 ( 2.5%)
# Score: 8286.0
# 
#
#=======================================

A_chicken_Vie      1 -------------------------AAAATGGAGAAAATAGTGCTTCTTC     25
                                              |||||||||||||||||||||||||
A_China_GD01_      1 AGCAAAAGCAGGGGTTCAATCTGTCAAAATGGAGAAAATAGTGCTTCTTC     50

A_chicken_Vie     26 TTGCAATAGTCAGCCTTGTCAAAAGCGATCAGATTTGCATTGGTTACCAT     75
                     |||||||||||||||||||.|||||.||||||||||||||||||||||||
A_China_GD01_     51 TTGCAATAGTCAGCCTTGTTAAAAGTGATCAGATTTGCATTGGTTACCAT    100

A_chicken_Vie     76 GCAAACAACTCGACAGAGCAGGTTGACACAATAATGGAAAAGAACGTTAC    125
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_    101 GCAAACAACTCGACAGAGCAGGTTGACACAATAATGGAAAAGAACGTTAC    150

A_chicken_Vie    126 TGTTACACATGCCCAAGACATACTGGAAAAGACACACAACGGAAAGCTCT    175
                     ||||||||||||||||||||||||||||||||||||||||||.|||||||
A_China_GD01_    151 TGTTACACATGCCCAAGACATACTGGAAAAGACACACAACGGGAAGCTCT    200

A_chicken_Vie    176 GCGATCTAGATGGAGTGAAGCCTCTGATTTTAAAAGATTGTAGTGTAGCT    225
                     |||||||||||||||||||||||||||||||||.||||||||||||||||
A_China_GD01_    201 GCGATCTAGATGGAGTGAAGCCTCTGATTTTAAGAGATTGTAGTGTAGCT    250

A_chicken_Vie    226 GGATGGCTCCTCGGAAACCCAATGTGTGACGAATTCATCAATGTGCCGGA    275
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_    251 GGATGGCTCCTCGGAAACCCAATGTGTGACGAATTCATCAATGTGCCGGA    300

A_chicken_Vie    276 ATGGTCTTACATAGTGGAGAAGGCCAATCCAGCCAATGACCTCTGTTACC    325
                     |||||||||||||||||||||||||||.||||||||||||||||||||||
A_China_GD01_    301 ATGGTCTTACATAGTGGAGAAGGCCAACCCAGCCAATGACCTCTGTTACC    350

A_chicken_Vie    326 CAGGGAATTTCAACGACTATGAAGAATTGAAACACCTATTGAGCAGAATA    375
                     ||||||||||||||||||||||||||.|||||||||||||||||||||||
A_China_GD01_    351 CAGGGAATTTCAACGACTATGAAGAACTGAAACACCTATTGAGCAGAATA    400

A_chicken_Vie    376 AACCATTTTGAGAAAATACAGATCATCCCCAAAAGTTCTTGGTCCGATCA    425
                     |||||||||||||||||.|||||||||.||||||||||||||||||||||
A_China_GD01_    401 AACCATTTTGAGAAAATTCAGATCATCTCCAAAAGTTCTTGGTCCGATCA    450

A_chicken_Vie    426 TGAAGCCTCATTAGGGGTGAGCTCAGCATGTCCATACCAGGGAAGTTCCT    475
                     |||||||||||.||||||||||||||||||||||||||||||||...|||
A_China_GD01_    451 TGAAGCCTCATCAGGGGTGAGCTCAGCATGTCCATACCAGGGAACGCCCT    500

A_chicken_Vie    476 CCTTTTTCAGAAATGTGGTATGGCTTATCAAAAAGAACAATGCATACCCA    525
                     |||||||||||||||||||||||||||||||||||||||||.||||||||
A_China_GD01_    501 CCTTTTTCAGAAATGTGGTATGGCTTATCAAAAAGAACAATACATACCCA    550

A_chicken_Vie    526 ACAATAAAGAGAAGCTACAATAATACCAACCAAGAAGATCTCTTGGTACT    575
                     ||||||||||||||||||||||||||||||||.||||||||.|||.||||
A_China_GD01_    551 ACAATAAAGAGAAGCTACAATAATACCAACCAGGAAGATCTTTTGATACT    600

A_chicken_Vie    576 GTGGGGGATTCACCATCCTAATGATGAGGCAGAGCAGACAGGGCTCTATC    625
                     ||||||.|||||.|||.|||||.|||.|||||||||||||..||||||||
A_China_GD01_    601 GTGGGGAATTCATCATTCTAATAATGCGGCAGAGCAGACAAAGCTCTATC    650

A_chicken_Vie    626 AAAACCCAACCACCTATATTTCCATTGGGACATCAACACTAAACCAGAGA    675
                     |||||||||||||||||||||||.|||||||||||||||||||||.||||
A_China_GD01_    651 AAAACCCAACCACCTATATTTCCGTTGGGACATCAACACTAAACCTGAGA    700

A_chicken_Vie    676 TTGGTACCAAAAATAGCCACTAGATCCAAAGTAAACGGGCAAAGTGGAAG    725
                     |||||||||||||||||.||||||||||||||||||||||||||||||||
A_China_GD01_    701 TTGGTACCAAAAATAGCTACTAGATCCAAAGTAAACGGGCAAAGTGGAAG    750

A_chicken_Vie    726 GATAGATTTCTTCTGGACAATTTTAAAACCGAATGATGCAATCAATTTTG    775
                     |||.|||||||||||||||||||||||||||||||||||||||||.||.|
A_China_GD01_    751 GATGGATTTCTTCTGGACAATTTTAAAACCGAATGATGCAATCAACTTCG    800

A_chicken_Vie    776 AGAGTAATGGAAATTTCATTGCTCCAGAATATGCATACAAAATTGTCAAG    825
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_    801 AGAGTAATGGAAATTTCATTGCTCCAGAATATGCATACAAAATTGTCAAG    850

A_chicken_Vie    826 AAAGGAGACTCAGCAATTATGAAAAGTGAAGTGGAATATGGTAACTGCAA    875
                     |||||.||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_    851 AAAGGGGACTCAGCAATTATGAAAAGTGAAGTGGAATATGGTAACTGCAA    900

A_chicken_Vie    876 CACCAAGTGTCAAACTCCAATGGGGGCGATAAACTCTAGTATGCCATTCC    925
                     |||||||||||||||||||||.||||||||||||||||||||||||||||
A_China_GD01_    901 CACCAAGTGTCAAACTCCAATAGGGGCGATAAACTCTAGTATGCCATTCC    950

A_chicken_Vie    926 ACAACATACACCCTCTCACCATCGGGGAATGTCCCAAATATGTGAAATCA    975
                     |||||||||||||||||||||||||||||||.||||||||||||||||||
A_China_GD01_    951 ACAACATACACCCTCTCACCATCGGGGAATGCCCCAAATATGTGAAATCA   1000

A_chicken_Vie    976 AACAAATTAGTCCTTGCGACTGGGCTCAGAAATAGCCCTCAAAGAGAGAG   1025
                     |||||||||||||||||||||||||||||||||||.||||.|||||||||
A_China_GD01_   1001 AACAAATTAGTCCTTGCGACTGGGCTCAGAAATAGTCCTCTAAGAGAGAG   1050

A_chicken_Vie   1026 AAGAAGAAAAAGAGGACTATTTGGAGCTATAGCAGGTTTTATAGAGGGAG   1075
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1051 AAGAAGAAAAAGAGGACTATTTGGAGCTATAGCAGGTTTTATAGAGGGAG   1100

A_chicken_Vie   1076 GATGGCAGGGAATGGTAGATGGTTGGTATGGGTACCACCATAGCAATGAG   1125
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1101 GATGGCAGGGAATGGTAGATGGTTGGTATGGGTACCACCATAGCAATGAG   1150

A_chicken_Vie   1126 CAGGGGAGTGGGTACGCTGCAGACAAAGAATCCACTCAAAAGGCAATAGA   1175
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1151 CAGGGGAGTGGGTACGCTGCAGACAAAGAATCCACTCAAAAGGCAATAGA   1200

A_chicken_Vie   1176 TGGAGTCACCAATAAGGTCAACTCGATCATTGACAAAATGAACACTCAGT   1225
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1201 TGGAGTCACCAATAAGGTCAACTCGATCATTGACAAAATGAACACTCAGT   1250

A_chicken_Vie   1226 TTGAGGCCGTTGGAAGGGAATTTAATAACTTAGAAAGGAGAATAGAGAAT   1275
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1251 TTGAGGCCGTTGGAAGGGAATTTAATAACTTAGAAAGGAGAATAGAGAAT   1300

A_chicken_Vie   1276 TTAAACAAGAAGATGGAAGACGGATTCCTAGATGTCTGGACTTATAATGC   1325
                     |||||||||||.||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1301 TTAAACAAGAAAATGGAAGACGGATTCCTAGATGTCTGGACTTATAATGC   1350

A_chicken_Vie   1326 TGAACTTCTGGTTCTCATGGAAAATGAGAGAACTCTAGACTTCCATGACT   1375
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1351 TGAACTTCTGGTTCTCATGGAAAATGAGAGAACTCTAGACTTCCATGACT   1400

A_chicken_Vie   1376 CAAATGTCAAGAACCTTTACGACAAGGTCCGACTACAGCTTAGGGATAAT   1425
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1401 CAAATGTCAAGAACCTTTACGACAAGGTCCGACTACAGCTTAGGGATAAT   1450

A_chicken_Vie   1426 GCAAAAGAGCTGGGTAACGGTTGTTTCGAGTTCTATCACAAATGTGATAA   1475
                     |||||.||.|||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1451 GCAAAGGAACTGGGTAACGGTTGTTTCGAGTTCTATCACAAATGTGATAA   1500

A_chicken_Vie   1476 CGAATGTATGGAAAGTGTAAGAAACGGAACGTATGACTACCCGCAGTATT   1525
                     .|||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1501 TGAATGTATGGAAAGTGTAAGAAACGGAACGTATGACTACCCGCAGTATT   1550

A_chicken_Vie   1526 CAGAAGAAGCAAGATTAAAAAGAGAGGAAATAAGTGGAGTAAAATTGGAA   1575
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1551 CAGAAGAAGCAAGATTAAAAAGAGAGGAAATAAGTGGAGTAAAATTGGAA   1600

A_chicken_Vie   1576 TCAATAGGAACTTACCAAATACTGTCAATTTATTCAACAGTGGCGAGTTC   1625
                     |||||||||||||||||||||||||||||||||||||||||.||||||||
A_China_GD01_   1601 TCAATAGGAACTTACCAAATACTGTCAATTTATTCAACAGTTGCGAGTTC   1650

A_chicken_Vie   1626 CCTAGTACTGGCAATCATGGTGGCTGGTCTATCTTTATGGATGTGCTCCA   1675
                     .||||.||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1651 TCTAGCACTGGCAATCATGGTGGCTGGTCTATCTTTATGGATGTGCTCCA   1700

A_chicken_Vie   1676 ATGGGTCGTTACAATGCAGAATTTGCATTTAAATTTGTGAGTTCAGATTG   1725
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_China_GD01_   1701 ATGGGTCGTTACAATGCAGAATTTGCATTTAAATTTGTGAGTTCAGATTG   1750

A_chicken_Vie   1726 TAGTTA--------------------   1731
                     ||||||                    
A_China_GD01_   1751 TAGTTAAAAACACCCTTGTTTCTACT   1776


#---------------------------------------
#---------------------------------------
```

```AC
########################################
# Program: needle
# Rundate: Mon  5 Apr 2021 18:38:52
# Commandline: needle
#    -auto
#    -stdout
#    -asequence emboss_needle-I20210405-183848-0488-84610877-p2m.aupfile
#    -bsequence emboss_needle-I20210405-183848-0488-84610877-p2m.bupfile
#    -datafile EDNAFULL
#    -gapopen 10.0
#    -gapextend 0.5
#    -endopen 10.0
#    -endextend 0.5
#    -aformat3 pair
#    -snucleotide1
#    -snucleotide2
# Align_format: pair
# Report_file: stdout
########################################

#=======================================
#
# Aligned_sequences: 2
# 1: A_chicken_Viet_Nam_10_2005_(H5N1)_segment_4
# 2: A_avian_Hong_Kong_719_2007_(H5N1)_segment_4
# Matrix: EDNAFULL
# Gap_penalty: 10.0
# Extend_penalty: 0.5
#
# Length: 1751
# Identity:    1681/1751 (96.0%)
# Similarity:  1681/1751 (96.0%)
# Gaps:          20/1751 ( 1.1%)
# Score: 8205.0
# 
#
#=======================================

A_chicken_Vie      1 -------------AAAATGGAGAAAATAGTGCTTCTTCTTGCAATAGTCA     37
                                  |||||||||||||||||||||||||||||||||.|||
A_avian_Hong_      1 GGTTCAATCCGTCAAAATGGAGAAAATAGTGCTTCTTCTTGCAATAATCA     50

A_chicken_Vie     38 GCCTTGTCAAAAGCGATCAGATTTGCATTGGTTACCATGCAAACAACTCG     87
                     |||||||.|||||.||||||||||||||||||||||||||||||||||||
A_avian_Hong_     51 GCCTTGTTAAAAGTGATCAGATTTGCATTGGTTACCATGCAAACAACTCG    100

A_chicken_Vie     88 ACAGAGCAGGTTGACACAATAATGGAAAAGAACGTTACTGTTACACATGC    137
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    101 ACAGAGCAGGTTGACACAATAATGGAAAAGAACGTTACTGTTACACATGC    150

A_chicken_Vie    138 CCAAGACATACTGGAAAAGACACACAACGGAAAGCTCTGCGATCTAGATG    187
                     .|||||.|||||||||||||||||||||||.|||||||||||||||||||
A_avian_Hong_    151 TCAAGATATACTGGAAAAGACACACAACGGGAAGCTCTGCGATCTAGATG    200

A_chicken_Vie    188 GAGTGAAGCCTCTGATTTTAAAAGATTGTAGTGTAGCTGGATGGCTCCTC    237
                     |||||||||||||||||||||.||||||||||||||||||||||||||||
A_avian_Hong_    201 GAGTGAAGCCTCTGATTTTAAGAGATTGTAGTGTAGCTGGATGGCTCCTC    250

A_chicken_Vie    238 GGAAACCCAATGTGTGACGAATTCATCAATGTGCCGGAATGGTCTTACAT    287
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    251 GGAAACCCAATGTGTGACGAATTCATCAATGTGCCGGAATGGTCTTACAT    300

A_chicken_Vie    288 AGTGGAGAAGGCCAATCCAGCCAATGACCTCTGTTACCCAGGGAATTTCA    337
                     |||||||||||||||.||||||||||||||||||||||||||||||||||
A_avian_Hong_    301 AGTGGAGAAGGCCAACCCAGCCAATGACCTCTGTTACCCAGGGAATTTCA    350

A_chicken_Vie    338 ACGACTATGAAGAATTGAAACACCTATTGAGCAGAATAAACCATTTTGAG    387
                     ||||||||||||||.|||||||||||||||||||.|||||||||||||||
A_avian_Hong_    351 ACGACTATGAAGAACTGAAACACCTATTGAGCAGGATAAACCATTTTGAG    400

A_chicken_Vie    388 AAAATACAGATCATCCCCAAAAGTTCTTGGTCCGATCATGAAGCCTCATT    437
                     |||||.|||||||||||||||||||||||||||||||||||||||||||.
A_avian_Hong_    401 AAAATTCAGATCATCCCCAAAAGTTCTTGGTCCGATCATGAAGCCTCATC    450

A_chicken_Vie    438 AGGGGTGAGCTCAGCATGTCCATACCAGGGAAGTTCCTCCTTTTTCAGAA    487
                     ||||||||||||||||||||||||||||||||...|||||||||||||||
A_avian_Hong_    451 AGGGGTGAGCTCAGCATGTCCATACCAGGGAACGCCCTCCTTTTTCAGAA    500

A_chicken_Vie    488 ATGTGGTATGGCTTATCAAAAAGAACAATGCATACCCAACAATAAAGAGA    537
                     |||||||||||||||||||||||||||||.||||||||||||||||||||
A_avian_Hong_    501 ATGTGGTATGGCTTATCAAAAAGAACAATACATACCCAACAATAAAGAGA    550

A_chicken_Vie    538 AGCTACAATAATACCAACCAAGAAGATCTCTTGGTACTGTGGGGGATTCA    587
                     ||||||||||||||||||||.||||||||.|||.||||||||||||||||
A_avian_Hong_    551 AGCTACAATAATACCAACCAGGAAGATCTTTTGATACTGTGGGGGATTCA    600

A_chicken_Vie    588 CCATCCTAATGATGAGGCAGAGCAGACAGGGCTCTATCAAAACCCAACCA    637
                     .|||.|||||||||..||||||||||||..||||||||||||||||||||
A_avian_Hong_    601 TCATTCTAATGATGCAGCAGAGCAGACAAAGCTCTATCAAAACCCAACCA    650

A_chicken_Vie    638 CCTATATTTCCATTGGGACATCAACACTAAACCAGAGATTGGTACCAAAA    687
                     |||||||||||.||||||||||||||||.|||||||||||||||||||||
A_avian_Hong_    651 CCTATATTTCCGTTGGGACATCAACACTGAACCAGAGATTGGTACCAAAA    700

A_chicken_Vie    688 ATAGCCACTAGATCCAAAGTAAACGGGCAAAGTGGAAGGATAGATTTCTT    737
                     |||||.|||||||||||||||||||||||||||||||||||.||||||||
A_avian_Hong_    701 ATAGCTACTAGATCCAAAGTAAACGGGCAAAGTGGAAGGATGGATTTCTT    750

A_chicken_Vie    738 CTGGACAATTTTAAAACCGAATGATGCAATCAATTTTGAGAGTAATGGAA    787
                     |||||||||||||||||||||||||||||||||.||.|||||||||||||
A_avian_Hong_    751 CTGGACAATTTTAAAACCGAATGATGCAATCAACTTCGAGAGTAATGGAA    800

A_chicken_Vie    788 ATTTCATTGCTCCAGAATATGCATACAAAATTGTCAAGAAAGGAGACTCA    837
                     |||||||||||||||||||||||||||||||||||||||||||.||||||
A_avian_Hong_    801 ATTTCATTGCTCCAGAATATGCATACAAAATTGTCAAGAAAGGGGACTCA    850

A_chicken_Vie    838 GCAATTATGAAAAGTGAAGTGGAATATGGTAACTGCAACACCAAGTGTCA    887
                     |||||||||||||||||.||||||||||||||||||||||||||||||||
A_avian_Hong_    851 GCAATTATGAAAAGTGAGGTGGAATATGGTAACTGCAACACCAAGTGTCA    900

A_chicken_Vie    888 AACTCCAATGGGGGCGATAAACTCTAGTATGCCATTCCACAACATACACC    937
                     |||||||||.||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    901 AACTCCAATAGGGGCGATAAACTCTAGTATGCCATTCCACAACATACACC    950

A_chicken_Vie    938 CTCTCACCATCGGGGAATGTCCCAAATATGTGAAATCAAACAAATTAGTC    987
                     |||||||||||||||||||.||||||||||||||||||||||||||||||
A_avian_Hong_    951 CTCTCACCATCGGGGAATGCCCCAAATATGTGAAATCAAACAAATTAGTC   1000

A_chicken_Vie    988 CTTGCGACTGGGCTCAGAAATAGCCCTCAAAGAGAGAGAAGAAGAAAAAG   1037
                     |||||||||||||||||||||||.||||.||||||.||||||||||||||
A_avian_Hong_   1001 CTTGCGACTGGGCTCAGAAATAGTCCTCTAAGAGAAAGAAGAAGAAAAAG   1050

A_chicken_Vie   1038 AGGACTATTTGGAGCTATAGCAGGTTTTATAGAGGGAGGATGGCAGGGAA   1087
                     ||||||||||||||||||||||||||||||||||||.|||||||||||||
A_avian_Hong_   1051 AGGACTATTTGGAGCTATAGCAGGTTTTATAGAGGGCGGATGGCAGGGAA   1100

A_chicken_Vie   1088 TGGTAGATGGTTGGTATGGGTACCACCATAGCAATGAGCAGGGGAGTGGG   1137
                     |||||||||||||||||||||..|||||||||||||||||||||||||||
A_avian_Hong_   1101 TGGTAGATGGTTGGTATGGGTTTCACCATAGCAATGAGCAGGGGAGTGGG   1150

A_chicken_Vie   1138 TACGCTGCAGACAAAGAATCCACTCAAAAGGCAATAGATGGAGTCACCAA   1187
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1151 TACGCTGCAGACAAAGAATCCACTCAAAAGGCAATAGATGGAGTCACCAA   1200

A_chicken_Vie   1188 TAAGGTCAACTCGATCATTGACAAAATGAACACTCAGTTTGAGGCCGTTG   1237
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1201 TAAGGTCAACTCGATCATTGACAAAATGAACACTCAGTTTGAGGCCGTTG   1250

A_chicken_Vie   1238 GAAGGGAATTTAATAACTTAGAAAGGAGAATAGAGAATTTAAACAAGAAG   1287
                     ||||||||||||||||||||||.||||||||||||||||||||||||||.
A_avian_Hong_   1251 GAAGGGAATTTAATAACTTAGAGAGGAGAATAGAGAATTTAAACAAGAAA   1300

A_chicken_Vie   1288 ATGGAAGACGGATTCCTAGATGTCTGGACTTATAATGCTGAACTTCTGGT   1337
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1301 ATGGAAGACGGATTCCTAGATGTCTGGACTTATAATGCTGAACTTCTGGT   1350

A_chicken_Vie   1338 TCTCATGGAAAATGAGAGAACTCTAGACTTCCATGACTCAAATGTCAAGA   1387
                     ||||||||||||||||||||||||||||||||||||.|||||||||||||
A_avian_Hong_   1351 TCTCATGGAAAATGAGAGAACTCTAGACTTCCATGATTCAAATGTCAAGA   1400

A_chicken_Vie   1388 ACCTTTACGACAAGGTCCGACTACAGCTTAGGGATAATGCAAAAGAGCTG   1437
                     |||||||||||||||||||||||||||||||||||||||||||.||||||
A_avian_Hong_   1401 ACCTTTACGACAAGGTCCGACTACAGCTTAGGGATAATGCAAAGGAGCTG   1450

A_chicken_Vie   1438 GGTAACGGTTGTTTCGAGTTCTATCACAAATGTGATAACGAATGTATGGA   1487
                     ||||||||||||||||||||||||||||||||||||||.|||||.|||||
A_avian_Hong_   1451 GGTAACGGTTGTTTCGAGTTCTATCACAAATGTGATAATGAATGCATGGA   1500

A_chicken_Vie   1488 AAGTGTAAGAAACGGAACGTATGACTACCCGCAGTATTCAGAAGAAGCAA   1537
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1501 AAGTGTAAGAAACGGAACGTATGACTACCCGCAGTATTCAGAAGAAGCAA   1550

A_chicken_Vie   1538 GATTAAAAAGAGAGGAAATAAGTGGAGTAAAATTGGAATCAATAGGAACT   1587
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1551 GATTAAAAAGAGAGGAAATAAGTGGAGTAAAATTGGAATCAATAGGAACT   1600

A_chicken_Vie   1588 TACCAAATACTGTCAATTTATTCAACAGTGGCGAGTTCCCTAGTACTGGC   1637
                     |||||||||||||||||||||||||||||.||||||||.||||.||||||
A_avian_Hong_   1601 TACCAAATACTGTCAATTTATTCAACAGTTGCGAGTTCTCTAGCACTGGC   1650

A_chicken_Vie   1638 AATCATGGTGGCTGGTCTATCTTTATGGATGTGCTCCAATGGGTCGTTAC   1687
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1651 AATCATGGTGGCTGGTCTATCTTTATGGATGTGCTCCAATGGGTCGTTAC   1700

A_chicken_Vie   1688 AATGCAGAATTTGCATTTAAATTTGTGAGTTCAGATTGTAGTTA------   1731
                     ||||||||||||||||||||||||||||||||||||||||||||      
A_avian_Hong_   1701 AATGCAGAATTTGCATTTAAATTTGTGAGTTCAGATTGTAGTTAAAAACA   1750

A_chicken_Vie   1732 -   1731
                      
A_avian_Hong_   1751 C   1751


#---------------------------------------
#---------------------------------------
```

```BC
########################################
# Program: needle
# Rundate: Mon  5 Apr 2021 18:40:19
# Commandline: needle
#    -auto
#    -stdout
#    -asequence emboss_needle-I20210405-184017-0218-29224839-p2m.aupfile
#    -bsequence emboss_needle-I20210405-184017-0218-29224839-p2m.bupfile
#    -datafile EDNAFULL
#    -gapopen 10.0
#    -gapextend 0.5
#    -endopen 10.0
#    -endextend 0.5
#    -aformat3 pair
#    -snucleotide1
#    -snucleotide2
# Align_format: pair
# Report_file: stdout
########################################

#=======================================
#
# Aligned_sequences: 2
# 1: A_China_GD01_2006_(H5N1)_segment_4
# 2: A_avian_Hong_Kong_719_2007_(H5N1)_segment_4
# Matrix: EDNAFULL
# Gap_penalty: 10.0
# Extend_penalty: 0.5
#
# Length: 1776
# Identity:    1731/1776 (97.5%)
# Similarity:  1731/1776 (97.5%)
# Gaps:          25/1776 ( 1.4%)
# Score: 8575.0
# 
#
#=======================================

A_China_GD01_      1 AGCAAAAGCAGGGGTTCAATCTGTCAAAATGGAGAAAATAGTGCTTCTTC     50
                                 |||||||||.||||||||||||||||||||||||||||
A_avian_Hong_      1 ------------GGTTCAATCCGTCAAAATGGAGAAAATAGTGCTTCTTC     38

A_China_GD01_     51 TTGCAATAGTCAGCCTTGTTAAAAGTGATCAGATTTGCATTGGTTACCAT    100
                     ||||||||.|||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_     39 TTGCAATAATCAGCCTTGTTAAAAGTGATCAGATTTGCATTGGTTACCAT     88

A_China_GD01_    101 GCAAACAACTCGACAGAGCAGGTTGACACAATAATGGAAAAGAACGTTAC    150
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_     89 GCAAACAACTCGACAGAGCAGGTTGACACAATAATGGAAAAGAACGTTAC    138

A_China_GD01_    151 TGTTACACATGCCCAAGACATACTGGAAAAGACACACAACGGGAAGCTCT    200
                     ||||||||||||.|||||.|||||||||||||||||||||||||||||||
A_avian_Hong_    139 TGTTACACATGCTCAAGATATACTGGAAAAGACACACAACGGGAAGCTCT    188

A_China_GD01_    201 GCGATCTAGATGGAGTGAAGCCTCTGATTTTAAGAGATTGTAGTGTAGCT    250
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    189 GCGATCTAGATGGAGTGAAGCCTCTGATTTTAAGAGATTGTAGTGTAGCT    238

A_China_GD01_    251 GGATGGCTCCTCGGAAACCCAATGTGTGACGAATTCATCAATGTGCCGGA    300
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    239 GGATGGCTCCTCGGAAACCCAATGTGTGACGAATTCATCAATGTGCCGGA    288

A_China_GD01_    301 ATGGTCTTACATAGTGGAGAAGGCCAACCCAGCCAATGACCTCTGTTACC    350
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    289 ATGGTCTTACATAGTGGAGAAGGCCAACCCAGCCAATGACCTCTGTTACC    338

A_China_GD01_    351 CAGGGAATTTCAACGACTATGAAGAACTGAAACACCTATTGAGCAGAATA    400
                     ||||||||||||||||||||||||||||||||||||||||||||||.|||
A_avian_Hong_    339 CAGGGAATTTCAACGACTATGAAGAACTGAAACACCTATTGAGCAGGATA    388

A_China_GD01_    401 AACCATTTTGAGAAAATTCAGATCATCTCCAAAAGTTCTTGGTCCGATCA    450
                     |||||||||||||||||||||||||||.||||||||||||||||||||||
A_avian_Hong_    389 AACCATTTTGAGAAAATTCAGATCATCCCCAAAAGTTCTTGGTCCGATCA    438

A_China_GD01_    451 TGAAGCCTCATCAGGGGTGAGCTCAGCATGTCCATACCAGGGAACGCCCT    500
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    439 TGAAGCCTCATCAGGGGTGAGCTCAGCATGTCCATACCAGGGAACGCCCT    488

A_China_GD01_    501 CCTTTTTCAGAAATGTGGTATGGCTTATCAAAAAGAACAATACATACCCA    550
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    489 CCTTTTTCAGAAATGTGGTATGGCTTATCAAAAAGAACAATACATACCCA    538

A_China_GD01_    551 ACAATAAAGAGAAGCTACAATAATACCAACCAGGAAGATCTTTTGATACT    600
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    539 ACAATAAAGAGAAGCTACAATAATACCAACCAGGAAGATCTTTTGATACT    588

A_China_GD01_    601 GTGGGGAATTCATCATTCTAATAATGCGGCAGAGCAGACAAAGCTCTATC    650
                     ||||||.|||||||||||||||.||||.||||||||||||||||||||||
A_avian_Hong_    589 GTGGGGGATTCATCATTCTAATGATGCAGCAGAGCAGACAAAGCTCTATC    638

A_China_GD01_    651 AAAACCCAACCACCTATATTTCCGTTGGGACATCAACACTAAACCTGAGA    700
                     ||||||||||||||||||||||||||||||||||||||||.||||.||||
A_avian_Hong_    639 AAAACCCAACCACCTATATTTCCGTTGGGACATCAACACTGAACCAGAGA    688

A_China_GD01_    701 TTGGTACCAAAAATAGCTACTAGATCCAAAGTAAACGGGCAAAGTGGAAG    750
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    689 TTGGTACCAAAAATAGCTACTAGATCCAAAGTAAACGGGCAAAGTGGAAG    738

A_China_GD01_    751 GATGGATTTCTTCTGGACAATTTTAAAACCGAATGATGCAATCAACTTCG    800
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    739 GATGGATTTCTTCTGGACAATTTTAAAACCGAATGATGCAATCAACTTCG    788

A_China_GD01_    801 AGAGTAATGGAAATTTCATTGCTCCAGAATATGCATACAAAATTGTCAAG    850
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    789 AGAGTAATGGAAATTTCATTGCTCCAGAATATGCATACAAAATTGTCAAG    838

A_China_GD01_    851 AAAGGGGACTCAGCAATTATGAAAAGTGAAGTGGAATATGGTAACTGCAA    900
                     |||||||||||||||||||||||||||||.||||||||||||||||||||
A_avian_Hong_    839 AAAGGGGACTCAGCAATTATGAAAAGTGAGGTGGAATATGGTAACTGCAA    888

A_China_GD01_    901 CACCAAGTGTCAAACTCCAATAGGGGCGATAAACTCTAGTATGCCATTCC    950
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    889 CACCAAGTGTCAAACTCCAATAGGGGCGATAAACTCTAGTATGCCATTCC    938

A_China_GD01_    951 ACAACATACACCCTCTCACCATCGGGGAATGCCCCAAATATGTGAAATCA   1000
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_    939 ACAACATACACCCTCTCACCATCGGGGAATGCCCCAAATATGTGAAATCA    988

A_China_GD01_   1001 AACAAATTAGTCCTTGCGACTGGGCTCAGAAATAGTCCTCTAAGAGAGAG   1050
                     |||||||||||||||||||||||||||||||||||||||||||||||.||
A_avian_Hong_    989 AACAAATTAGTCCTTGCGACTGGGCTCAGAAATAGTCCTCTAAGAGAAAG   1038

A_China_GD01_   1051 AAGAAGAAAAAGAGGACTATTTGGAGCTATAGCAGGTTTTATAGAGGGAG   1100
                     ||||||||||||||||||||||||||||||||||||||||||||||||.|
A_avian_Hong_   1039 AAGAAGAAAAAGAGGACTATTTGGAGCTATAGCAGGTTTTATAGAGGGCG   1088

A_China_GD01_   1101 GATGGCAGGGAATGGTAGATGGTTGGTATGGGTACCACCATAGCAATGAG   1150
                     |||||||||||||||||||||||||||||||||..|||||||||||||||
A_avian_Hong_   1089 GATGGCAGGGAATGGTAGATGGTTGGTATGGGTTTCACCATAGCAATGAG   1138

A_China_GD01_   1151 CAGGGGAGTGGGTACGCTGCAGACAAAGAATCCACTCAAAAGGCAATAGA   1200
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1139 CAGGGGAGTGGGTACGCTGCAGACAAAGAATCCACTCAAAAGGCAATAGA   1188

A_China_GD01_   1201 TGGAGTCACCAATAAGGTCAACTCGATCATTGACAAAATGAACACTCAGT   1250
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1189 TGGAGTCACCAATAAGGTCAACTCGATCATTGACAAAATGAACACTCAGT   1238

A_China_GD01_   1251 TTGAGGCCGTTGGAAGGGAATTTAATAACTTAGAAAGGAGAATAGAGAAT   1300
                     ||||||||||||||||||||||||||||||||||.|||||||||||||||
A_avian_Hong_   1239 TTGAGGCCGTTGGAAGGGAATTTAATAACTTAGAGAGGAGAATAGAGAAT   1288

A_China_GD01_   1301 TTAAACAAGAAAATGGAAGACGGATTCCTAGATGTCTGGACTTATAATGC   1350
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1289 TTAAACAAGAAAATGGAAGACGGATTCCTAGATGTCTGGACTTATAATGC   1338

A_China_GD01_   1351 TGAACTTCTGGTTCTCATGGAAAATGAGAGAACTCTAGACTTCCATGACT   1400
                     ||||||||||||||||||||||||||||||||||||||||||||||||.|
A_avian_Hong_   1339 TGAACTTCTGGTTCTCATGGAAAATGAGAGAACTCTAGACTTCCATGATT   1388

A_China_GD01_   1401 CAAATGTCAAGAACCTTTACGACAAGGTCCGACTACAGCTTAGGGATAAT   1450
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1389 CAAATGTCAAGAACCTTTACGACAAGGTCCGACTACAGCTTAGGGATAAT   1438

A_China_GD01_   1451 GCAAAGGAACTGGGTAACGGTTGTTTCGAGTTCTATCACAAATGTGATAA   1500
                     ||||||||.|||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1439 GCAAAGGAGCTGGGTAACGGTTGTTTCGAGTTCTATCACAAATGTGATAA   1488

A_China_GD01_   1501 TGAATGTATGGAAAGTGTAAGAAACGGAACGTATGACTACCCGCAGTATT   1550
                     ||||||.|||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1489 TGAATGCATGGAAAGTGTAAGAAACGGAACGTATGACTACCCGCAGTATT   1538

A_China_GD01_   1551 CAGAAGAAGCAAGATTAAAAAGAGAGGAAATAAGTGGAGTAAAATTGGAA   1600
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1539 CAGAAGAAGCAAGATTAAAAAGAGAGGAAATAAGTGGAGTAAAATTGGAA   1588

A_China_GD01_   1601 TCAATAGGAACTTACCAAATACTGTCAATTTATTCAACAGTTGCGAGTTC   1650
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1589 TCAATAGGAACTTACCAAATACTGTCAATTTATTCAACAGTTGCGAGTTC   1638

A_China_GD01_   1651 TCTAGCACTGGCAATCATGGTGGCTGGTCTATCTTTATGGATGTGCTCCA   1700
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1639 TCTAGCACTGGCAATCATGGTGGCTGGTCTATCTTTATGGATGTGCTCCA   1688

A_China_GD01_   1701 ATGGGTCGTTACAATGCAGAATTTGCATTTAAATTTGTGAGTTCAGATTG   1750
                     ||||||||||||||||||||||||||||||||||||||||||||||||||
A_avian_Hong_   1689 ATGGGTCGTTACAATGCAGAATTTGCATTTAAATTTGTGAGTTCAGATTG   1738

A_China_GD01_   1751 TAGTTAAAAACACCCTTGTTTCTACT   1776
                     |||||||||||||             
A_avian_Hong_   1739 TAGTTAAAAACAC-------------   1751


#---------------------------------------
#---------------------------------------
```

(Did you remember to add your name to this Markdown file?)
