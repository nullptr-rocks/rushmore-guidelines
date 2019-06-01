# Principles



## The Zen of Python ( for C++ too )

- Beautiful is better than ugly.
- Explicit is better than implicit.
- Simple is better than complex.
- Complex is better than complicated.
  Flat is better than nested.
- Sparse is better than dense.
- Readability counts.
- Special cases aren't special enough to break the rules.
- Although practicality beats purity.
  Errors should never pass silently.
- Unless explicitly silenced.
- In the face of ambiguity, refuse the temptation to guess.
- There should be one - and preferably only one - obvious way to do it.
- Although that way may not be obvious at first unless you're Dutch.
- Now is better than never.
- Although never is often better than *right* now.
- If the implementation is hard to explain, it's a bad idea.
- If the implementation is easy to explain, it may be a good idea.
- Namespaces are one honking great idea - let's do more of those!



## Usability and Discoverability

*Developers are human too.* 

*We got tired.* 

*We forget.* 

*We are weak.*



Why do we continue to make the things difficult for ourselves? May be a problematic sense of pride or maybe we are unprepared. In ether case, this must stop as soon as possible. When coding something for other human being use, always remember to think more like a designer than a tech wizard. The work magic terms are *Usability* and *Discoverability*.

Adapted from the Nielsen Norman Group articles about usability:

> Usability is a *quality attribute* that assesses how easy *interfaces* are to use. The word "usability" also refers to methods for improving ease-of-use during the *design process*.
>
> Usability is defined by these components:
>
> * Learnable: Easy first access to the basic tasks.
> * Efficient: Seasoned users must be able to perform better.
> * Memorable: The interface sticks in the mind before some time.
> * Errors: Severe errors are difficult to happens and mild ones are easy to recover.
> * Satisfaction: The tool is pleasant to use.



Pay attention to the important terms disclosed here: quality attribute, interfaces and design process. Wherever you are designing an interface, always exercise judgment based on the components listed above. 

Discoverability is the average rate a user can discover and learn new features. In the case of code, how easy is to discover a feature merely interacting with the system without documentation.

But as Scott Berkun disclaimed in [The Myth of Discoverability](https://scottberkun.com/essays/26-the-myth-of-discoverability/):

> You can not make every **SINGLE** word stand out.

What do we learn?

*Prioritize the convenience of the essentials and emphasize the most important parts of the interface. Reduce steps when possible and use familiar mechanisms to make the semantics clear. The lesser and more specialized parts don’t need to be overly discoverable as the interested user will have the documentation in this cases. But always make sure to let the basics shine.* 



## Determinism

There are cases non-deterministic algorithms are better. But they are always difficult to implement right. Also non-determinism is difficult to understand in general. For practical reasons, I encourage the use of strictly deterministic solutions. 

The exception is external modules and plug-ins where this behavior is isolated to the internals of the system. Well known libraries are also allowed as their behaviors is battle-tested. 



## Openly Multi-paradigmatic

I abhor the old *“mine is better than yours”* attitude. There is no such thing as the perfect programming language or paradigm. What really exist is cases and situations something is better applicable. We cannot forget people have right to like or dislike anything at they hearts content. That said, I hope everyone joining this project to be open-minded about using the tools that are convenient for the work. I’ll not advocate for a pure object-oriented, functional, procedural or any other paradigm under the sun as the base of this project. 

It is very likely to be a multi-paradigmatic project and if you join us, I hope you like this scenario.



## Game Programming = Creative Programming

What Game programming is not:

- Systems Developent
- Web Development
- Applications Development
- Research and Development
- Embedded Systems
- OS

Game Programming is all about expressing a game idea through code. The area related to the use of programming to creative expression is called Creative Programming. In particular, Game Programming can be seen as a superset of Creative Programming aiming to complex behaviors and interactivity. So, stay away from any overly convoluted solutions that can harm the usability of the system and aim to high expressibility.



## Worse is better

### Simplicity

The design must be simple, both in implementation and interface. It is more important for the implementation to be simple than the interface. **Simplicity is the most important consideration in a design**.

### Correctness

The design should be correct in all observable aspects, but **It is slightly better to be simple than correct**.

### Consistency

**The design must not be overly inconsistent**. Consistency can be sacrificed for simplicity in some cases, but it is better to drop those parts of the design that deal with less common circumstances than to introduce either complexity or inconsistency in the implementation.

### Completeness

The design must cover as many important situations as is practical. All reasonably expected cases should be covered. **Completeness can be sacrificed in favor of any other quality**. In fact, completeness must be sacrificed whenever implementation simplicity is jeopardized. Consistency can be sacrificed to achieve completeness if simplicity is retained; especially worthless is consistency of interface.

