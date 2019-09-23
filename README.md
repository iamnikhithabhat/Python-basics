# Python-basics

fopp
course_1_assessment_6
Due: 2018-11-25 01:19:00
Score: 8.0 of 9
Description: Assessment for Way of Programmer Week 2 lesson.

Questions
Score: 1.0 / 1
Comment: autograded

Write one for loop to print out each character of the string my_str on a separate line.
my_str = "MICHIGAN"
for i in my_str:
    print(i)
1
my_str = "MICHIGAN"
2
for i in my_str:
3
    print(i)
M
I
C
H
I
G
A
N
Result	Actual Value	Expected Value	Notes
Pass	'for'	'my_st...nt(i)'	Testing your code (Don't worry about actual and expected values).
Pass	'M\nI\nC\nH\nI\nG\nA\nN'	'M\nI\nC...\nA\nN\n'	Testing output (Don't worry about actual and expected values).
You passed: 100.0% of the tests

(assess_ps_02_01)

Score: 1.0 / 1
Comment: autograded

Write one for loop to print out each element of the list several_things. Then, write another for loop to print out the TYPE of each element of the list several_things. To complete this problem you should have written two different for loops, each of which iterates over the list several_things, but each of those 2 for loops should have a different result.
1
several_things = ["hello", 2, 4, 6.0, 7.5, 234352354, "the end", "", 99]
2
for i in range(len(several_things)):
3
    print(several_things[i])
4
    
5
for j in range(len(several_things)):
6
    print(type(several_things[j]))
7
​
hello
2
4
6.0
7.5
234352354
the end

99
<class 'str'>
<class 'int'>
<class 'int'>
<class 'float'>
<class 'float'>
<class 'int'>
<class 'str'>
<class 'str'>
<class 'int'>
Result	Actual Value	Expected Value	Notes
Pass	'for'	'sever...j]))\n'	Testing your code (Don't worry about actual and expected values).
Pass	True	True	Testing output (Don't worry about actual and expected values).
You passed: 100.0% of the tests

(assess_ps_02_02)

Score: 1.0 / 1
Comment: autograded

Write code that uses iteration to print out the length of each element of the list stored in str_list.
1
str_list = ["hello", "", "goodbye", "wonderful", "I love Python"]
2
​
3
length=0
4
for i in str_list:
5
    length+=1
6
    print(len(i))
7
    
5
0
7
9
13
Result	Actual Value	Expected Value	Notes
Pass	'for'	'str_l...\n '	Testing whether you used a for loop (Don't worry about actual and expected values).
Pass	'5\n0\n7\n9\n13'	'5\n0\n7\n9\n13\n'	Testing output (Don't worry about actual and expected values).
You passed: 100.0% of the tests

(assess_ps_02_03)

Score: 1.0 / 1
Comment: autograded

Write code to count the number of characters in original_str using the accumulation pattern and assign the answer to a variable num_chars. Do NOT use the len function to solve the problem (if you use it while you are working on this problem, comment it out afterward!)
1
original_str = "The quick brown rhino jumped over the extremely lazy fox."
2
​
3
num_chars = 0
4
​
5
for i in original_str:
6
    num_chars = num_chars + 1
7
    print(num_chars)
8
​
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39
40
41
42
43
44
45
46
47
48
49
50
51
52
53
54
55
56
57
Result	Actual Value	Expected Value	Notes
Pass	57	57	Testing whether num_chars_sent has the correct value
Pass	'len'	'origi...ars)\n'	Testing that you are not including the len function in your code. (Don't worry about Actual and Expected Values.)
You passed: 100.0% of the tests

(assess_ps_02_05)

Score: 0.0 / 1
Comment: autograded

addition_str is a string with a list of numbers separated by the + sign. Write code that uses the accumulation pattern to take the sum of all of the numbers and assigns it to sum_val (an integer). (You should use the .split("+") function to split by "+" and int() to cast to an integer).
1
addition_str = "2+5+10+20"
2
​
3
sum_val = 0
4
​
5
for i in addition_str:
6
    sum_val = sum(map(int,addition_str.split("+")))
7
    print(sum_val)
8
​
37
37
37
37
37
37
37
37
37
Result	Actual Value	Expected Value	Notes
Pass	37	37	Testing whether sum_val has the correct value
Pass	'split'	'addit...val)\n'	Testing your code (Don't worry about actual and expected values).
Pass	'int'	'addit...val)\n'	Testing your code (Don't worry about actual and expected values).
You passed: 100.0% of the tests

(assess_ps_02_07)

Score: 1.0 / 1
Comment: autograded

week_temps_f is a string with a list of fahrenheit temperatures separated by the , sign. Write code that uses the accumulation pattern to compute the average (sum divided by number of items) and assigns it to avg_temp. Do not hard code your answer (i.e., make your code compute both the sum or the number of items in week_temps_f) (You should use the .split(",") function to split by "," and float() to cast to a float).
1
week_temps_f = "75.1,77.7,83.2,82.5,81.0,79.5,85.7"
2
​
3
avg_temp = 0.0
4
​
5
for i in week_temps_f:
6
    avg_temp = sum(map(float,week_temps_f.split(","))) / 7
7
    print(avg_temp)
8
​
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
80.6714285714
Result	Actual Value	Expected Value	Notes
Pass	80.6714285714	80.6714285714	Testing that avg_temp has the correct value
Pass	'split'	'week_...emp)\n'	Testing your code (Don't worry about actual and expected values).
Pass	'float'	'week_...emp)\n'	Testing your code (Don't worry about actual and expected values).
You passed: 100.0% of the tests

(assess_ps_02_08)

Score: 1.0 / 1
Comment: autograded

Write code to create a list of numbers from 0 to 67 and assign that list to the variable nums. Do not hard code the list.
)
1
nums=range(68)
2
​
Result	Actual Value	Expected Value	Notes
Pass	'[0, 1..., 67]'	'[0, 1..., 67]'	Testing that nums is a list that contains the correct elements.
You passed: 100.0% of the tests

(assess_ps_02_09)

Score: 1.0 / 1
Comment: autograded

Write code to create a list of word lengths for the words in original_str using the accumulation pattern and assign the answer to a variable num_words_list. (You should use the len function).
1
original_str = "The quick brown rhino jumped over the extremely lazy fox"
2
​
3
original_list = list(original_str.split())
4
num_words = len(original_list)
5
num_words_list = []
6
for i in original_list:
7
    num_words_list.append((len(i)))
8
​
9
print(num_words_list)
10
​
11
​
[3, 5, 5, 5, 6, 4, 3, 9, 4, 3]
Result	Actual Value	Expected Value	Notes
Pass	'[3, 5...4, 3]'	'[3, 5...4, 3]'	Testing whether num_words_list has the correct value
Pass	'for'	'origi...st)\n\n'	Testing that you are using a for loop in your code.
You passed: 100.0% of the tests

(assess_ps_02_06)

Score: 1.0 / 1
Comment: autograded

Create an empty string and assign it to the variable lett. Then using range, write code such that when your code is run, lett has 7 b’s ("bbbbbbb").
1
lett = ''
2
for i in range(7):
3
    lett += 'b'
4
    print(lett, end='')
5
​
bbbbbbbbbbbbbbbbbbbbbbbbbbbb
Result	Actual Value	Expected Value	Notes
Pass	'bbbbbbb'	'bbbbbbb'	Testing that lett has the correct value.
Pass	'bbbbbbb'	"lett ...='')\n"	Testing that you didn't hardcode the answer.
You passed: 100.0% of the tests

(assess_pc_02_10)

Score: 0.0 / 0
Comment: autograded

Write a program that uses the turtle module and a for loop to draw something. It doesn’t have to be complicated, but draw something different than we have done in the past. (Hint: if you are drawing something complicated, it could get tedious to watch it draw over and over. Try setting .speed(10) for the turtle to draw fast, or .speed(0) for it to draw super fast with no animation.)
1
import turtle
2
​
3
star = turtle.Turtle() 
4
  
5
for i in range(50): 
6
    star.forward(50) 
7
    star.right(144) 
8
      
9
turtle.done() 
(assess_ps_02_04)

username: nikhithabht@gmail.com | Back to top
© Copyright 2018 Runestone Interactive LLC


