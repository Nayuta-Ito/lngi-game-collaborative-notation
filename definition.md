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
d(x)=c(c(...(x)...)))

## The dawn of array
### Source
https://discord.com/channels/589829547667619852/589939910442614795/703151445775745026
### Definition
[x]y where [1]y = ay, [2]y = by, [3]y = cy, and [x+1]y = [x][x][x]...[x]y (with y x's)

## 2 entries Part 1
### Source
https://discord.com/channels/589829547667619852/594679014703235072/828287186653937665
### Definition
[0,1]n =[n]n

## 2 entries Part 2
### Source
https://discord.com/channels/589829547667619852/594679014703235072/838499801188270101
(and a few later posts)
### Definition
[n,1]m = [n-1,1]^m m for any integers n>=1 and m>=1

## 2 entries Part 3
### Source
https://discord.com/channels/589829547667619852/594679014703235072/840362470346063872

### Definition
[0,m]n = [n,m-1]

## 3+ linear entries
### Source
https://discord.com/channels/589829547667619852/594679014703235072/850792842707206145
https://discord.com/channels/589829547667619852/594679014703235072/850805890705653800

"the combined message to pin"
https://discord.com/channels/589829547667619852/594679014703235072/850956034390360064

### Definition
Once we reach the limit of two entries, can we expand this notation to 3+ entires in the following:
z represents an empty array or 1 or more zeroes.
\# can be anything
[z,0,a+1,#]n = [z,n,a,#]n
[a+1,#]n = [a,#]^n(n)
[#,z]n = [#]n

## Nested array definition
### Source
https://discord.com/channels/589829547667619852/901168147934117888/911352758936961034

### Definition
1. [z(b+1,#)a+1...]n (where # represents the rest of the dimensional seperator or can be empty) = [z(b,#)0(b,#)...0(b,#)0(b,#)1(b+1,#)a...]n with n (b,#)'s
2. [...(A)z(B)a...]n = [...(B)a...] if the level of A is less than the level of B.
3. if a seperator begins with 0 and has more than 1 entry, jump into it and set n to the n of the main array.
4. (0) is the comma and rules from previous parts apply.

Note that z can only contain zeroes and seperators. 

## Slash
### Source
https://discord.com/channels/589829547667619852/1000504288231043143/1071279268706914455
Amendment: Done on GitHub, with the branch `slash_amendment` with PR#3

### Definition
```
[b#]x = "[b-1#]"^x x
[Z0(c#)b@]x = [Z0(c-1#) "0(c-1#)"^x-1 b@]x
[Z0(#c/0)b@]x = [Z0(#c)b@]x
[Z[1]0(Z[2]c#)b]x = [Z[1]0(Z[2]c#)b...
[Z0(Z'0/b...y/z@)1%]x = [Z0(Z'0(...(Z'1/b-1...y/z@)...)b...y/z@)%]x,  with x sets of parens.
```

where:
```
Z,Z' = zero array, #@% are arrays
For bcxyz, the output is always bigger than 0 
```
