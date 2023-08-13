## A
### Source
https://discord.com/channels/589829547667619852/594679014703235072/594847931643723797
### Definition
Rule 1: Use 'a' instead of 'e' for this one... idk

## B
### Source
https://discord.com/channels/589829547667619852/594679014703235072/594994335624331299
(nobody agreed it)
### Definition
xb = a^x

Before here, b was posts fix.
https://discord.com/channels/589829547667619852/594679014703235072/625791108387045412

## C
### Source
https://discord.com/channels/589829547667619852/589939910442614795/625793309625024547
### Definition
c(a) = (10)bb...bb (with a b's)

## D
### Source
https://discord.com/channels/589829547667619852/589939910442614795/697223684976279552
### Definition
d(x)=c(c(...(10)...)))

## The dawn of arrays
### Source
https://discord.com/channels/589829547667619852/589939910442614795/703151445775745026
### Definition
[x]y where [1]y = ay, [2]y = by, [3]y = cy, and [x+1]y = [x][x][x]...[x]10 (with y x's)

## 2 entries I
### Source
https://discord.com/channels/589829547667619852/594679014703235072/828287186653937665
### Definition
[0,1]n =[n]10

## 2 entries II
### Source
https://discord.com/channels/589829547667619852/594679014703235072/838499801188270101
(and a few later posts)
### Definition
[n,1]m = [n-1,1]^m 10 for any integers n>=1 and m>=1

## 2 entries III
### Source
https://discord.com/channels/589829547667619852/594679014703235072/840362470346063872

### Definition
[0,m]n = [n,m-1]10

## Linear
### Source
https://discord.com/channels/589829547667619852/594679014703235072/850792842707206145
https://discord.com/channels/589829547667619852/594679014703235072/850805890705653800

"the combined message to pin"
https://discord.com/channels/589829547667619852/594679014703235072/850956034390360064

### Definition
Once we reach the limit of two entries, can we expand this notation to 3+ entires in the following:
z represents an empty array or 1 or more zeroes.
\# can be anything
[z,0,a+1,#]n = [z,n,a,#]10
[a+1,#]n = [a,#]^n 10
[#,z]n = [#]n

## Dimensional
### Source
https://discord.com/channels/589829547667619852/901168147934117888/911352758936961034

### Definition
1. [z(b+1,#)a+1...]n (where # represents the rest of the dimensional seperator or can be empty) = [z(b,#)0(b,#)...0(b,#)0(b,#)1(b+1,#)a...]10 with n (b,#)'s
2. [...(A)z(B)a...]n = [...(B)a...] if the level of A is less than the level of B.
3. If a seperator begins with 0 and has more than 1 entry, jump into it and set n to the n of the main array.
4. (0) is the comma and rules from previous parts apply.

Note that z can only contain zeroes and seperators. 

## Slash
### Source
https://discord.com/channels/589829547667619852/1000504288231043143/1071279268706914455
Amendment: Done on GitHub, with the branch `slash_amendment` with PR#3
Revision: Done on Github

### Definition

1. [a#]x = "[a-1 #]"^x 10
2. [z 0(b@)a #]x = [z "0(b-1 @)"^x 1(b @)a-1 #]10
3. When we have [z(y 0/b @)a...]n, it becomes [z X<sub>n</sub> 1(y 0/b @)a-1...]10, where
   3.1. If y is empty, then X<sub>0</sub> = (0/b-1 @)
   3.2. Otherwise X<sub>0</sub> = (y/1/b-1).
   3.3. X<sub>a</sub> = (x/0 X<sub>a-1</sub> 1/b-1).
4. When we have [z 0(0\#)a @]n, then change it to [z 0**(0\#)**1(0\#)a-1 @]n and jump into the bolded separator.

where:  
x, y and z are zero arrays, # and @ are arrays, and
the values of a, b, and c are all bigger than zero.


## Dimensional slash
### Source
Github, by solarzone

### Definition

1. [a#]x = "[a-1 #]"^x 10
2. [z 0(b@)? a #]x = [z "0 (b-1 @)?"^x 1 (b @)? a-1 #]10
3. When we have [z(x y 0/b <span>$</span>)a...]n, it becomes [z X<sub>n</sub> a...]10, where  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3.1. x' and <span>$</span> are as short as possible  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3.2. If y is empty, then X<sub>0</sub> = (x (0/b)? <span>$</span>)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3.3. Otherwise X<sub>0</sub> = (x (y 1/b-1)? <span>$</span>).  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3.4. To calculate X<sub>a</sub>,  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3.4.1. Start at the outermost level of (x y 0/b <span>$</span>), so we have (Z 0(@)? a #). Change this to (Z 0(@)? 1 (@)? a-1 #).  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3.4.2. Then, jump into (@) and do it again. Do this until we reach (Z 0/a #), at which point stop.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3.4.3. Then we have (x' y 0/b <span>$</span>'), for some x' and <span>$</span>'. X<sub>a</sub> = (x' y 0 X<sub>a-1</sub> 1/b-1 <span>$</span>').  
4. When we have [z 0(0#)? a @]n, then change it to \[z 0 **(0#)?** 1(0#)? a-1 @\]n and jump into the bolded separator.

where:  
The / separator is an abbreviation for (0)/,  
x, y and z are zero arrays, # and @ are arrays, <span>$</span> and <span>$</span>' are strings,  
? is either empty or /, and the values of a, b, and c are all bigger than zero.

