# Project proposal

## The user and a language

This section describes who the project would serve and why a language might be a
good way to meet their needs.

The project would serve anyone that works with "words". Linguists, Archivists, Scrabble players, or anyone looking for anagrams in their own name (/j).  
It is not limited to this domain of experts though. The features provided could be useful to anyone, for instance - if you would like to perform a more complex "ctrl-f" on a document. 

Programming languages allow users to build systems and automate certain tasks. Linguists already use PLs, but these do not have the features or fluency that meet the goals of a linguist. A DSL would help because the way a string works for most people - and how a string works for linguists is different. And making a new language would help create different datatypes that allow different types of strings of characters behave differently. ("lorem", `lorem', ^lorem^ - all contain the same "string of characters" but they would have different behavior and functions associated to them.)

Linguists, anagramists, archivists, scrabble players - use programs and codes all the time, but it is more cumbersome due to the limitations of strings, and datatypes and operations. And the fact that most PLs only have one string type. 


### What's the need?

_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help
them?_

The language would give the user some new datatypes, that are similar to strings in appearance but have different functionality. (they are strings of characters, but a different datatype by virtue of different functionality)

This helps linguists, or any people that work with words, for whom different words behave differently (IPA, Romanization systems, sound shifts, anagrams, reduplication, etc.). 
Performing some simple operations can be cumbersome, and a bit of a roadblock towards building larger linguistic helper tools, or even models. This would make things easier. 

Beyond that, the features of additional string manipulation can be used by anyone. For instance, if someone wants to perform a complex "ctrl+f" on an piece of text. Not a straightforward ctrl-f, but more like "any word than contains a number in it" or something like that. Not the best example, but the point is - when you want to do a more detailed search in a text. You could control the environment of the word you are looking for, a feature of a word, or some set of variation of a word.


### Why a language?

_Why is a DSL appropriate for your user(s)? How does it address the need?_

Programming languages allow users to build systems and automate certain tasks. Linguists already use PLs to study sound shift, cognates, etc. A DSL allows some specialization, and the introduction of new forms of loops and datatypes that would help performing linguistic operations and string manipulation.

A DSL allows you to redefine the workings of somethings. For instance, if the user defines "or" to be equal to "our", then just a simple 
("color" == "colour") or ("behaviour" == behavior") should both result in true for a particular string type. 

Some new datatypes will be more similar to strings, while others are not. An example of one that is similar, but not exactly the same is the IPA-String. It holds IPA values, which are also a string of symbols but act slightly differently. For instance "tʃ" are two seperate symbols, but produce a single sound when together - and linguists treat it as a single length character. So performing a ".length()" should treat these two symbols as one. Currently, a programmer would have to program a seperate "if" statement where they look for "t" followed by "ʃ" in each string, and substract one from the length each time this is seen. This is cumbersome. And this needs to be repeated for any forseeable affricate and dipthong. A new string, with a new "length" would solve this. This is only one example of one difference in IPA-Strings.

Numbers already have many different types - double, int, long, etc.

### Why you?

_What excites you about this idea? How did you come up with it?_

This excites my because I really enjoy linguistics and words.  My neurodivergent brain also loves scrabble, anagrams, and such - and the programming language provides tools for those too. Beyond that, I feel like this project would be fun to program because we are using a lot of the techniques we learnt in class. Such as multiple lists, implicit conversion, and addition of operators. 


### Domain

_Describe the project's domain in five words._

New character manipulations for linguists.

### Interface (syntax)

_How might the user interact with the language? What does programming look
like? Why is this the right way to interact with the problem domain?_

It would work much like any other PL. You write the program, run it - it can take text based inputs and outputs. The domain deals largely with words, so it makes sense that the user interact with it via a text-based console.

### Operation (semantics)

_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

The program will perform operations as guided by the programmer, on the input piece of text. The output will contain a little more information about the word being output. This extra information will be displayed in paranthesis. The input and output will both be done via the console. 
Type errors would be easy to make in this DSL, because these is a lot of character based types. These errors will be communicated to the user via the console. 

The input, output, and errors are all text based. The program is too. The DSL will look like a weird, twisted form of Scala. 

### Expressiveness

_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

Working with words, sentences and any form of text should be easy. There is a lot of string matching and string operation tools. And the new loop structure will be built around it. 

Several existing operations will be used for other purposes, so doing what was originally intended for those operations might be a little bit harder. 

Anything that falls outside of Turing completeness will obviously be impossible.

### Related work

_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

I could not find any in this domain, and I think it is because most linguists just use the single string data type, and the provided loops and operations, to make their desired program. But there is a lot of room for abstraction, and a lot of room for improvement by adding new types and operators. 

I looked up linguistic DSLs, and a list of DSLs, and I asked ChatGPT - and they all drew blanks. I could not find anything similar to this. [this is intentional though. My previous idea already existed, so I switched to this idea. I chose this idea BECAUSE there were no DSLs in this exact domain]

## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

Language design is really important here, because idea itself is to make it easier for string manipulation. The design is necessarily important. Also, the new datatypes look like strings ("lorem"), but have different functionality. So it is important to make the distinction intuitive. The new loops, types, operations, and conversions must all be easy to remember and use. 

The systems aspect has some work too, but there isn't any particularly complicated semantics. 

### Scope

_How big an idea is this? How ambitious is this project?_

It is a very reasonable size, in my opinion. The idea involves a lot of functions, implicit conversions, and claseses - but most of these techniques, we have learnt in class before and - this is just an extension of that. We also created a new loop syntax with the internal DSL lab/puzzles. So while the idea itself has a lot of features, most of it feels doable because we have implemented similar techniques in class before.  

### Benefits and drawbacks

_Why might this be a good idea for a project? Why might this not be a good idea
project?_

I think it is a good idea because: 

- I am doing a linguistics concentration, and I am quite passionate about it, so I think I would be passionate about this project. I would also have enough insite into the domain. 
- The DSL feels like something I myself would use.
- It allows me to use a lot of the different tools, techniques and fluency we learnt in class. 
