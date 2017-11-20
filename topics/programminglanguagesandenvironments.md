What Is ... a Programming Language?
===

## Summary

A programming language is a constructed language that is readable by humans, but interuptritable by computers. Each language has its own vocabulary and set of grammatical rules that instruct computers to execute a set of defined instructions.

![Generic](https://media.giphy.com/media/10zxDv7Hv5RF9C/giphy.gif 'generic')

Each language has two main components it's *syntax* and it's *functions*. These are important as they can differ language to language.

### Why do we need programming languages?

So a computer is a hive of electrical signals, which are almost always On / Off signals (or sequences of). 

![moss](https://media.giphy.com/media/13HgwGsXF0aiGY/giphy.gif 'moss')

It is these signals that make the machine perform tasks. If we were to write a word processing application using just these On / Off signals ... well it wouldnt be a pleasurable experience. This is where programming languages are useful, they allow us to abstract these On / Off signals into Human Readable language thereby simplifying the writing process.

You can split languages into two levels: Low and High.
The levels refer to the amount of abstraction from machine code. 

Assembly and Machine Code are both examples of a low level language. 

High level languages are things like C, C++, Java, PHP, Python etc.

Below is an example from [Wikipedia](https://en.wikipedia.org/wiki/Low-level_programming_language) which is the same function that generates the next number of the ***Fibonacci Sequence*** in three different languages from Low to High level.

**Machine Code**

~~~
8B542408 83FA0077 06B80000 0000C383
FA027706 B8010000 00C353BB 01000000
B9010000 008D0419 83FA0376 078BD989
C14AEBF1 5BC3
~~~

**Assembly**

~~~
fib:
    mov edx, [esp+8]
    cmp edx, 0
    ja @f
    mov eax, 0
    ret
    
    @@:
    cmp edx, 2
    ja @f
    mov eax, 1
    ret
    
    @@:
    push ebx
    mov ebx, 1
    mov ecx, 1
    
    @@:
        lea eax, [ebx+ecx]
        cmp edx, 3
        jbe @f
        mov ebx, ecx
        mov ecx, eax
        dec edx
    jmp @b
    
    @@:
    pop ebx
    ret
~~~

**C**

~~~
unsigned int fib(unsigned int n) {
    if (n <= 0)
        return 0;
    else if (n <= 2)
        return 1;
    else {
        unsigned int a,b,c;
        a = 1;
        b = 1;
        while (1) {
            c = a + b;
            if (n <= 3) return c;
            a = b;
            b = c;
            n--;
        }
    }
}
~~~

You should have a look at some assembly just to appreciate how amazing the language is. You constantly hear people ***'you have more computing power in your pocket than what went to the moon'***. And they are correct. However, what they don't say is how the hardware was programmed. 

Here is [Apollo 11s' Guidance Computer](https://github.com/chrislgarry/Apollo-11/).

### Which Language is best ... ?

There are a alot of languages ... 

![Languages](../images/languages.gif "Languages")

and it's not a competition, we should really ask **What language would be best for ...?**

Some of the more useful languages and a good place to start.

Language | Description
--- | --- 
**Java** | General Purpose Language that is used for desktop, mobile and tablet applications. It works on all platforms. 
**Javascript** | One of the most widely used languages. Can be used to make games, websites, applications and server systems.
**C** | Compiled procedural language. Useful for system programming.
**C++** | General Purpose Language. Extremely powerful, is used to make system software, game engines / games, desktop, web and mobile applications.
**C#** | Very similar to Java (Considered a modern day Java).
**ObjectiveC** | General Purpose Language used by Apple for desktop and mobile applications.
**Python** | High Level General Purpose Language. It is simple, readable and makes a solid foundation for a number of uses such as data science, embedded applications and some desktop apps. (A good starter language)
**PHP** | Server Side Programming Language. 
**Swift** | Successor to ObjectiveC
**SQL** | Database Language.

For more details on other languages check [wikipedia](https://en.wikipedia.org/wiki/List_of_programming_languages).

## IDE

An Integrated Development Environment usually refers to an application that handles writing, compiling and running the coded program.  

For Example:

* [XCode](https://developer.apple.com/xcode/)
* [Microsoft Visual Studio](https://www.visualstudio.com/)
* [NetBeans](https://netbeans.org/)
* [Xamarin](https://www.xamarin.com/)
* [Eclipse](https://www.eclipse.org/)
* [Codeblocks](http://www.codeblocks.org/)
* [QT Editor](https://www.qt.io/)

These programmes make it easier for developer to create applications and systems.

### Other Editors

Whilst an IDE offers an integrated approach to coding. Sometimes programmers want to use a more lightweight editor that make it easier to edit code.

For Example:

* [Sublime](https://www.sublimetext.com/)
* [Atom](https://atom.io/)
* [Text Wrangler](https://itunes.apple.com/gb/app/textwrangler/id404010395?mt=12)
* [BBEdit](https://www.barebones.com/products/bbedit/)
* [Visual Studio Code](https://code.visualstudio.com/)

## Gotcha

HTML and CSS are not programming languages. They are markup languages.

## Useful Resources

* [The Different Uses of Programming Languages](https://9gag.com/gag/aDwN219/the-different-uses-of-programming-languages)
* [Programming Resource](http://programming-motherfucker.com/become.html)
* [Codecademy](https://www.codecademy.com/) great place to learn new languages.
* [Mashable](http://mashable.com/2014/01/21/learn-programming-languages/#OuiGgabTSaqB)
* [openFrameworks](http://openframeworks.cc/)
* [Processing](https://processing.org/)