# Conventions

Coding is difficult. Any programmer with more than a few years in this industry will tell you that. Coding with other people adds the complexity of social relations. Open-source is beautiful, but we know it can get really messy, really fast.

Ladies and Gentleman, let's us do a contract of sorts. I build this guide to anyone wanting to get involved with this project and myself. I ask to everyone interested in coding for this project to abide to this rules as much as possible. 

> This rules can change and if you find something unreasonable, it's open to discussion with every major contributor.



## C++

###  0 - Guidelines

It would be wasteful to simply toss the work of people much more brilliant than me doing a complete new set of rules. The genius of Bjarne Stroustrup and Herb Sutter gave us the *C++ Core Guidelines*  and I intend to use them. So:

> This project respects the C++ Core Guidelines as much as possible. If you intend to give us a hand, please do it too.

The C++ Core Guidelines are found at  https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines 

There is one exception to this rule:

*The rule NL.26 is ignored and superseded by the always-on-the-right const. To know why, please visit the [East const Central](http://slashslash.info/eastconst/).*



### 1 - Disabled Features

The following features must be disabled and are not used in any part of the code for this project:

* Run-time type information
* Exceptions
* dynamic_cast

### 2 - Documentation

**On comments:** 

The comments must be written in clear english and use *Doxygen* markings. Each header file must have a *header comment block*. This is useful for the end user, but also for the system developer. The following must have comment:

- Classes and Structs
- Unions
- Enumerations
- Free functions
- Public constants, variables and methods
- Protected constants, variables and methods
- Alias (using or typedef)
- Class and method templates 

Private constants, variables and methods are optionally commented. But as a rule of thumb, It is an effective way to keep the code more esoteric behavior explained. 

Keep the comments brief and focused. If it is not possible, it must be one of two things: 

- The interface/code is bloated - In such case, refactoring carefully may be interesting.
- The system has high complexity or very low-level - In this case, the system must be explained in a separate markdown file to be referred in the comment.

The template comments are available on [comments](comments.md)

### 3 - Style

Style is largely a tool to help the developer to concentrate in the code. There is no true style, but a choice had to be made. The style chosen is the [Juce Style](https://juce.com/discover/stories/coding-standards).  

The clang-format style file is found as [juce.clang-format](style/juce.clang-format).

### 4 - Automated Analysis

It is never to much work to be safe. Nobody likes to use a faulty piece of software or stay late fixing such software. To reduce the possibility of these happenings, we use automated analysis tools.

- PVS-Studio Analyzer - Scan and fix before commit.
- Clang tools: clang-tidy, clang-format, modularize, clang-include-fixer
- include-what-you-use

### 5 - Unit Tests

We use TDD for most of the cases. As a rule of thumb:

- Create a header file and write the public interfaces you intend to use.
- Comment all obligatory parts of the interface. Try to explain the intended behavior of all methods and functions.
- Create the tests using the behaviors you described on the comments.
- Create a implementation file.
- Start coding.

The test library used is: [doctest](https://github.com/onqtam/doctest)

### 6 - Coverage

We use coveralls. If the project don’t have a coveralls file already,  you are free to do it yourself.



## Python

[PEP8](https://www.python.org/dev/peps/pep-0008/) all the way.



## Go

```bash
run gofmt
```

The implication are made clear [here](https://github.com/golang/go/wiki/CodeReviewComments).