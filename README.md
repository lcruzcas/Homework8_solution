#   Autograder-grading explanation (Homework # 8): 

In general students will have three possible outcomes pushed back to their repositories for each problem.
* Test Passed 
* Test Case # Timed out 
* Test Failed #

## Test # 1 (20 points) ##
```
from os import listdir
from os.path import isfile, join, splitext

directory='lecs'
path = join(directory, '13_vidText.txt')
ro=read_and_clean_doc(path)
print(ro)
```
## Test # 2 (16 points) ##
```
from os import listdir
from os.path import isfile, join, splitext
import numpy

directory='lecs'
path1 = join(directory, '9_vidText.txt')
path2 = join(directory, '13_vidText.txt')
path3 = join(directory, '7_vidText.txt')
path4 = join(directory, '4_vidText.txt')
path5 = join(directory, '12_vidText.txt')
path6 = join(directory, '1_vidText.txt')
doclist =[path1, path2, path3, path4,path5,path6]

dw,wl=build_doc_word_matrix(doclist)
print( dw[0], dw[1], dw[2],dw[3], dw[4], dw[5], wl)
```
## Test # 3 (16 points) ##
```
from os import listdir
from os.path import isfile, join, splitext

directory='lecs'
path1 = join(directory, '9_vidText.txt')
path2 = join(directory, '13_vidText.txt')
path3 = join(directory, '7_vidText.txt')
path4 = join(directory, '4_vidText.txt')
path5 = join(directory, '12_vidText.txt')
path6 = join(directory, '1_vidText.txt')
doclist =[path1, path2, path3, path4,path5,path6]
dw,wl=build_doc_word_matrix(doclist)
tf=build_tf_matrix(dw)

#print(tf[0], tf[1], tf[2],tf[3],tf[4],tf[5])
```
## Test # 4 (16 points) ##
```
from os import listdir
from os.path import isfile, join, splitext

directory='lecs'
path1 = join(directory, '9_vidText.txt')
path2 = join(directory, '13_vidText.txt')
path3 = join(directory, '7_vidText.txt')
path4 = join(directory, '4_vidText.txt')
path5 = join(directory, '12_vidText.txt')
path6 = join(directory, '1_vidText.txt')
doclist =[path1, path2, path3, path4,path5,path6]
dw,wl=build_doc_word_matrix(doclist)
tf=build_tf_matrix(dw)

#print(tf)
```
## Test # 5 (16 points) ##
```
from os import listdir
from os.path import isfile, join, splitext

directory='lecs'
path1 = join(directory, '9_vidText.txt')
path2 = join(directory, '13_vidText.txt')
path3 = join(directory, '7_vidText.txt')
path4 = join(directory, '4_vidText.txt')
path5 = join(directory, '12_vidText.txt')
path6 = join(directory, '1_vidText.txt')
doclist =[path1, path2, path3, path4,path5,path6]
dw,wl=build_doc_word_matrix(doclist)
tf=build_tf_matrix(dw)
#print(tf[0], tf[1], tf[2], tf[3],tf[4], tf[5])
```
## Test # 5 (16 points) ##
```
from os import listdir
from os.path import isfile, join, splitext

directory='lecs'
path1 = join(directory, '9_vidText.txt')
path2 = join(directory, '13_vidText.txt')
path3 = join(directory, '7_vidText.txt')
path4 = join(directory, '4_vidText.txt')
path5 = join(directory, '12_vidText.txt')
path6 = join(directory, '1_vidText.txt')
doclist =[path1, path2, path3, path4,path5,path6]
dw,wl=build_doc_word_matrix(doclist)
tf=build_tf_matrix(dw)
student=find_distinctive_words(dw,wl,doclist)
#print(student)
```

