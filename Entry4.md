# Learning how to use context free grammars
Up until this point, the way I would've had something like the calculator function would be taking the two terms, and then the operation being performed all as
seperate inputs to try to avoid any nasty bugs around sanitizing the inputs or breaking up the string to find all the components of the equation.
Once we learned about context free grammars in class, I was ecstatic at the prospect of all the time not having to worry about this for my calculator assignment, however that was short lived
as initially, I had some trouble setting up and using context free garmmars and understanding how to use them.


## Attempting to make sense of it
Understanding that parsing was the foundation of all of this really helped clear alot of this up. Parsing it self seemed simple enough, it is just how(in the case of the calculator)
the computer proccesses the input. What stumped me though was how what this did was any different then what the context free grammar did.  
This [youtube video](https://www.youtube.com/watch?v=vXZ92lYOeIw&ab_channel=MiftaSintaha) in particular was extremely helpful in my understanding of context free grammars

## The fog is slowly clearing
Eventually, after doing some additional research, I came to understand that context free grammars are...very aptly named. As what they do is essentially the same as the function of
grammar rules in the english language. When a context free grammar(again in the case of the calculator) defines how to interpret what a "+" means, it is the same as saying "ok the word
code is pronounced like 'ko-hd' and not 'co-dey'" in english.

## Finding the purpose
Once again, the english language example came to the rescue. Essentially I realized, context-free grammars are to parsing what knowing the definition of a word is to learning how to read it. 
Without the knowledge of what the word means, its just a bunch of letters next to eachother. You know that this word has the letters C, O, D, and E in it, but they are just as 
meaningless totally meaningless without knowing what the word "code" is referring to(essentially the step parsing takes in interpreting the user input), knowing what the letters mean when you
put them together, is the role of the context free grammar in interpreting user input. 
