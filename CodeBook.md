## CodeBook <br \>

## Overview of the merged tidy dataset <br \>

>str(merge.all) <br \>

\## 'data.frame':    10299 obs. of  563 variables: <br \>
\##  $ subjectID                           : int  1 1 1 1 1 1 1 1 1 1 ... <br \>
\##  $ activityID                          : int  5 5 5 5 5 5 5 5 5 5 ... <br \>
\##  $ tBodyAcc-mean()-X                   : num  0.289 0.278 0.28 0.279 0.277 ... <br \>
\##  $ tBodyAcc-mean()-Y                   : num  -0.0203 -0.0164 -0.0195 -0.0262 -0.0166 ... <br \>
\##  $ tBodyAcc-mean()-Z                   : num  -0.133 -0.124 -0.113 -0.123 -0.115 ... <br \>
\##  $ tBodyAcc-std()-X                    : num  -0.995 -0.998 -0.995 -0.996 -0.998 ... <br \>
\##  $ tBodyAcc-std()-Y                    : num  -0.983 -0.975 -0.967 -0.983 -0.981 ... <br \>
\##  $ tBodyAcc-std()-Z                    : num  -0.914 -0.96 -0.979 -0.991 -0.99 ... <br \>
\##  $ tBodyAcc-mad()-X                    : num  -0.995 -0.999 -0.997 -0.997 -0.998 ... <br \>
\##  $ tBodyAcc-mad()-Y                    : num  -0.983 -0.975 -0.964 -0.983 -0.98 ... <br \>
\##  $ tBodyAcc-mad()-Z                    : num  -0.924 -0.958 -0.977 -0.989 -0.99 ... <br \>
\##  $ tBodyAcc-max()-X                    : num  -0.935 -0.943 -0.939 -0.939 -0.942 ... <br \>
\##  $ tBodyAcc-max()-Y                    : num  -0.567 -0.558 -0.558 -0.576 -0.569 ... <br \>
\##  $ tBodyAcc-max()-Z                    : num  -0.744 -0.818 -0.818 -0.83 -0.825 ... <br \>
\##  $ tBodyAcc-min()-X                    : num  0.853 0.849 0.844 0.844 0.849 ... <br \>
\##  $ tBodyAcc-min()-Y                    : num  0.686 0.686 0.682 0.682 0.683 ... <br \>
\##  $ tBodyAcc-min()-Z                    : num  0.814 0.823 0.839 0.838 0.838 ... <br \>
\##  $ tBodyAcc-sma()                      : num  -0.966 -0.982 -0.983 -0.986 -0.993 ... <br \>
\##  $ tBodyAcc-energy()-X                 : num  -1 -1 -1 -1 -1 ... <br \>
\##  $ tBodyAcc-energy()-Y                 : num  -1 -1 -1 -1 -1 ... <br \>
\##  $ tBodyAcc-energy()-Z                 : num  -0.995 -0.998 -0.999 -1 -1 ... <br \>

## Variables Listing <br \>

>colnames(merge.all) <br \>

\##   [1] "subjectID"                           
\##   [2] "activityID"                         
\##   [3] "tBodyAcc-mean()-X"                    
\##   [4] "tBodyAcc-mean()-Y"                    
\##   [5] "tBodyAcc-mean()-Z"                   
\##   [6] "tBodyAcc-std()-X"                     
\##   [7] "tBodyAcc-std()-Y"                     
\##   [8] "tBodyAcc-std()-Z"                     
\##   [9] "tBodyAcc-mad()-X"                     
\##  [10] "tBodyAcc-mad()-Y"                     
\##  [11] "tBodyAcc-mad()-Z"                     
\##  [12] "tBodyAcc-max()-X"                     
\##  [13] "tBodyAcc-max()-Y"                     
\##  [14] "tBodyAcc-max()-Z"                     
\##  [15] "tBodyAcc-min()-X"                     
\##  [16] "tBodyAcc-min()-Y"                     
\##  [17] "tBodyAcc-min()-Z"                     
\##  [18] "tBodyAcc-sma()"                       
\##  [19] "tBodyAcc-energy()-X"                  
\##  [20] "tBodyAcc-energy()-Y"                  
\##  [21] "tBodyAcc-energy()-Z"         

## Overview of the independent second tidy datasets <br \>

>str(secdata) <br \>

\## 'data.frame':    180 obs. of  82 variables: <br \>
\##  $ subjectID                      : int  1 2 3 4 5 6 7 8 9 10 ... <br \>
\##  $ activityID                     : int  1 1 1 1 1 1 1 1 1 1 ... <br \>
\##  $ activityType                   : Factor w/ 6 levels "LAYING","SITTING",..: 4 4 4 4 4 4 4 4 4 4 ... <br \>
\##  $ tBodyAcc-mean()-X              : num  0.277 0.276 0.276 0.279 0.278 ... <br \>
\##  $ tBodyAcc-mean()-Y              : num  -0.0174 -0.0186 -0.0172 -0.0148 -0.0173 ... <br \>
\##  $ tBodyAcc-mean()-Z              : num  -0.111 -0.106 -0.113 -0.111 -0.108 ... <br \>
\##  $ tBodyAcc-std()-X               : num  -0.284 -0.424 -0.36 -0.441 -0.294 ... <br \>
\##  $ tBodyAcc-std()-Y               : num  0.1145 -0.0781 -0.0699 -0.0788 0.0767 ... <br \>
\##  $ tBodyAcc-std()-Z               : num  -0.26 -0.425 -0.387 -0.586 -0.457 ... <br \>
\##  $ tGravityAcc-mean()-X           : num  0.935 0.913 0.937 0.964 0.973 ... <br \>
\##  $ tGravityAcc-mean()-Y           : num  -0.2822 -0.3466 -0.262 -0.0859 -0.1004 ... <br \>
\##  $ tGravityAcc-mean()-Z           : num  -0.0681 0.08473 -0.13811 0.12776 0.00248 ... <br \>
\##  $ tGravityAcc-std()-X            : num  -0.977 -0.973 -0.978 -0.984 -0.979 ... <br \>
\##  $ tGravityAcc-std()-Y            : num  -0.971 -0.972 -0.962 -0.968 -0.962 ... <br \>
\##  $ tGravityAcc-std()-Z            : num  -0.948 -0.972 -0.952 -0.963 -0.965 ... <br \>

