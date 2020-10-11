# How I came to understand Haskell/Functional Programming

At the beginning of the course, I was EXTREMELY confused. I thought to myself, "this is so unlike any programming language I've ever touched before, what can I do with this".
To a beginner, the style and method of operating haskell seems very foreign and confusing, however, after many failed attempts, I was able to break it down into discrete parts
that helped me gain a basic understanding of how to write code in haskell!


### Putting it in terms I know
One of the biggest things that helped me understand the flow of programming in a functional language, compared to the imparative ones I had used exclusively up until this point,
was to take basic operations and compare and contrast how they work in the two types of languages. 
In an imparative language, multiplying 3*2 is as simple as just using the multiplication function, however in haskell and other functional languages, we have to think of it on
a more basic level. We have to think about it as what math is involved in multiplying 3 and 2.  
In the case of a simple function like multiplication, it is just adding 3+3!  

### Analogies to the rescue!
Finding real world examples analogous to how functional programming languages worked was essential to my understanding. From my background in game design, I was able to come up with one that
really explained it well.  
So lets say in a video game, I have a player and I want a player to take damage when they run into an enemy. In an imperative programming language, I would simply say:  
`If player collides with enemy, player takes damage`  
In a functional language, however, we need to go deeper then that. In the case of the player for example, we need to define the parameters of what it does.  
Lets define the player as "A character that can walk around the world controlled by the person playing the game, the player has 3 health that will deplete when it gets hurt".
This isnt enough though, we need to define exactly WHAT walking is.  
In the case of the walking example, we would have to go as far as to say "On a key press, the player moves forward X distance", and even then, we have to go further and define
what a key press is, and what forward is.  
This is like functional programming in that we cant simply say "Multiply 3 by 2" like we would in an imperative language. We have to go further and define
exactly multiplication is, and say "We add 3 to itself two times", then after that we need to define what ADDITION is. The process repeats itself until there are no more processes left to define.
Once we figure out everything we need to define, we start at the lowest level and build up from there!

Since last feburary, I have been interning at a Video Game company working as a game designer, part of my job is writing up designs for new game systems and the most important aspect of those
documents is digging into every little detail and level of abstraction of what exactly I want and how exactly this new system should behave. Realizing the similarities between that and functional programming really
helped me understand exactly what I need to accomplish when working with a language like Haskell.
