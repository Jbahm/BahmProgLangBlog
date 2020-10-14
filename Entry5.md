# Learning Lambda Calculus
A reoccuring theme these blog entries has been explaining how I came to understand a certain topic in this course. When deciding what to write my blogs on, I decided on
doing them in this style because I figured this is the kind of resource/style of explanation that I would be looking for if I had to learn these topics from scratch.
That being said, the next one I want to investigate is how I learned to write and interpret Lambda Calculus notation.  


## Seems easy enough...
On the most basic tier of function, writing in lambda calculus notation is simple enough. It is merely just replacing f(x) with λx. Really nothing that was too hard to understand at all.

## Diving Deeper
Functions with one and even two variables in them are simple enough too. The only real added step is that in a function (λx.λy.x+y)1 2, you would sub in the variables one at a time.
The original equation would turn into (λx.λy.1+y)2, and then even further, it would reduce down to 1+2! Where it starts to really get tricky is when you have to substitute in other variables.

## Renaming variables
Up until this point with lambda calculus, I really hadn't found myself struggling too much with using it. Which was SHOCKING to me because so far in this class, understanding the major
concepts has required some amount of extra effort. Inevitably, lambda calculus found its way onto that list, and the thing I had the most difficulty with understanding was when it came to renaming variables.
The biggest stumbling block here was that in my head, I was vastly over-complicating it. The way I went about solving that issue was just going step by step and trying to understand what the equation was doing.  
For example, on the equation `(λx, M)N` I realized all I was acutally doing was replacing the variable M with the variable N. 

## But why?
The other issue i was having trouble understanding with replacing/renaming parameters was why exactly we were doing it. The confusion though, came more from overcomplicating it,
and it was as simple as thinking in terms of code. So say we have two variables, both named 'y'. If i try to assign something to y, the computer would get confused as it wouldnt know
which 'y' to assign it to. This is where the renaming comes in, it is simply a matter of changing the name for functionalities sake.
