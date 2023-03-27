# Project proposal

## The user and a language

This section describes who the project would serve and why a language might be a
good way to meet their needs.

The project would serve anyone that works with "words". Linguists, Archivists, Scrabble players, or anyone looking for anagrams in their own name (/j).  
It is not limited to this domain of experts though. The features provided could be useful to anyone, for instance - if you would like to perform a more complex "ctrl-f" on a document. 

Language would be a good way to meet their needs, because the way a string works for most people - and how a string works for linguists is different. And making a new language would help create different datatypes that allow different types of strings of characters behave differently. ("lorem", `lorem', ^lorem^ - all contain the same "string of characters" but they would have different behavior and functions associated to them)

Linguists, anagramists, archivists, scrabble players - use programs and code all the time, but it is more cumbersome due to the limitations of string. And the presence of only one form of string in most languages.


### What's the need?

_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help
them?_

The language would give the user some new datatypes, that are similar to strings in appearance but have different functionality. 

This helps people that work with words, for whom different words behave differently (IPA, Romanization systems, sound shifts, anagrams, reduplication, etc.). 
Performing some simple operations can be cumbersome, and a bit of a roadblock towards building larger linguistic helper tools, or even models. This would make things easier. 

Beyond that, the features of additional string manipulation can be used by anyone. For instance, if someone wants to perform a "ctrl+f" on an piece of text but instead of a straight forward ctrl-f, it is more like "any word than contains a number in it" or something like that. Not the best example, but the point is - when you want to do a more detailed search in a text.


### Why a language?

_Why is a DSL appropriate for your user(s)? How does it address the need?_

Programming languages allow users to build systems and automate certain tasks. Linguists already use PLs, but these do not have the features or fluency that meet the goals of a linguist. A DSL allows some specialization, and the introduction of new forms of loops and datatypes that would help performing linguistic operations and string manipulation.

A DSL allows you to redefine the workings of somethings. For instance, if the user defines "or" to be equal to "our", then just a simple 
("color" == "colour") or ("behaviour" == behavior") should both result in true. 

### Why you?

_What excites you about this idea? How did you come up with it?_

This excites my because I really enjoy linguistics and words.  My neurodivergent brain also loves scrabble, anagrams, and such - and the programming language provides tool for those too. Beyond that, I feel like this project would be fun to program because we are using a lot of the techniques we learnt in class. Such as multiple lists, and addition of operators. 


### Domain

_Describe the project's domain in five words._

New string manipulation for linguists.

### Interface (syntax)

_How might the user interact with the language? What does programming look
like? Why is this the right way to interact with the problem domain?_

It would work much like any other PL. You write the program, run it - it can take text based inputs and outputs. 

### Operation (semantics)

_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

The program will perform operations as guided by the programmer, on the input piece of text. The output will contain a little more information about the word being outputted. 
Type errors would be easy to make in this DSL, and these errors will be communicated to the user via the console.

### Expressiveness

_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

Working with words, sentences and any form of text should be easy. There is a lot of string matching. 
Several operations will be used for other purposes, so doing what was originally intended for those operations might be a little bit harder. 
Anything that falls outside of Turing completeness will obviously be impossible.

### Related work

_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

Language design is really important here, because most of it is to make it easier for string manipulation. The new datatypes look like strings ("lorem"), but have different functionality. So it is important to make the distinction intuitive. The new loops, operations, and conversions must all be easy to remember and use. 

The systems aspect has some work too, but there isn't any particularly complicated semantics. 

### Scope

_How big an idea is this? How ambitious is this project?_

It is a very reasonable size, in my opinion. There are a lot of functions, implicit conversions, and types - but most of these techniques, we have learnt in class before and - this is just an extension of that. We also created a new loop syntax in internal DSL lab. So while the idea itself has a lot of features, most of it feels doable because we have implemented similar techniques in class before.  

### Benefits and drawbacks

_Why might this be a good idea for a project? Why might this not be a good idea
project?_

I think it is a good idea because: 

- I am doing a linguistics concentration, and I am quite passionate about it, so I think I would be passionate about this project and I would have enough insite into the domain. 
- The DSL feels like something I myself would use.
- It allows me to use a lot of the different tools and fluency we learnt in class. 
