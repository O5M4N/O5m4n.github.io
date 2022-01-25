---
title: "Basics for Computer-Networking"
layout: page
categories: [Computer-Networking]
tags: [Computer-networking, Binary Decimal]
---
<br>
In this post I will try to explain the
Basic operations we will use for subnetting.

## conversions
- [Binary to Decimal](https://o5m4n.github.io/Basic-Computer-Networking#binary-to-decimal)
- [Decimal to Binary](https://o5m4n.github.io/Basic-Computer-Networking#decimal-to-binary)
<br>  
<br>  

### Binary to Decimal


The decimal number is equal to the sum of binary digits (dn) times their power of 2 (2n).

For networking we will use the table down below 

**Reference table**  

| 2<sup>7</sup>| 2<sup>6</sup> | 2<sup>5</sup> | 2<sup>4</sup> | 2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup>| 2<sup>0</sup> |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |  

<br />
**Example:**  
convert 101101  
we set each 1 from right to left 

<div class="table-wrapper" markdown="block">
  
| 2<sup>7</sup>| 2<sup>6</sup> | 2<sup>5</sup> | 2<sup>4</sup> | 2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup>| 2<sup>0</sup> | Number |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |     |
|     |     | 1   | 0   | 1   | 1   | 0   | 1   | BIN |
| 0   | 0   | 32  | 0   | 8   | 4   | 0   | 1   | 45  |
  
</div>  
we add the value of each result together to get **45**  

  
<br />   
### Decimal to Binary

**Reference table**  

| 2<sup>7</sup>| 2<sup>6</sup> | 2<sup>5</sup> | 2<sup>4</sup> | 2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup>| 2<sup>0</sup> |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |  

<br />
**Example:**  
convert 78  
we compare 78 to every value on table.

<pre>
78 >= 128 = No 
78 >= 64  = YES -> 78 - 64 = 14  
14 >= 32  = NO  
14 >= 16  = NO  
14 >= 8   = YES -> 14 - 8  = 6
6  >= 4   = YES -> 6  - 4  = 2
2  >= 2   = YES -> 2  - 2  = 0
0  >= 1   = NO
</pre>

we replace every yes by 1 on reference table  

| 2<sup>7</sup>| 2<sup>6</sup> | 2<sup>5</sup> | 2<sup>4</sup> | 2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup>| 2<sup>0</sup> |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
| 0   | 1   | 0   | 0   | 1   | 1   | 1   | 0   |  

**78 = 01001110**


<br>
