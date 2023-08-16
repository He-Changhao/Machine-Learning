Dataset: Pols1973

Description: 
It contains the first three formant frequency values and levels from the 12 Dutch monophthong vowels as spoken in /h_t/ context by 50 male speakers. 
The first three columns in the table contain the frequencies of the first three formants in Hertz and the next three columns contain the levels of the formants in decibel below the overall sound pressure level (SPL) of the measured vowel segment. 

Pols1973.mat:
The speech data is stored in the "Pols1973.mat" file. This file contains two variables: "fea" and "gnd". The 'fea' variable is a matrix of size (600, 6) where each row represents a sample. The 'gnd' variable corresponds to the label associated with each sample.

There are twelve types of labels in 'gnd':
['u ' 'a ' 'o ' '\as' '\o/' 'i ' 'y ' 'e ' '\yc' '\ep' '\ct' '\ic'], I'm not sure if this is correct because I don't understand Dutch either.



Reference:
Pols, L. C. W., Tromp, H. R. C., & Plomp, R. (1973). Frequency analysis of Dutch vowels from 50 male speakers. The Journal of the Acoustical Society of America, 53(4), 1093-1101.