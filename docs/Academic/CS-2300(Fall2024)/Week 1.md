### What is Discrete Math?

Discrete math is a branch of mathematics that employs unique tools and disciplines like logic, graph theory, and combinatorics to analyze objects with a finite nature. These tools have practical applications in computer science


### Notes for Module 1

Logic is formal reasoning with an emphasis on making precise statements.

#Propositions are statements that are either true or false. They are the most basic element in logic.

Questions are not propositions, but propositions can be an answer to a question.

A proposition has a truth value which can be true, false, unknown, or some value in between (like an opinion)

Important variables:

Zybooks refers to p, q, r for our variables as opposed to x, y, z. It doesn't really matter but each set of mathematics has its own unique set of symbols, even if they're somewhat analogous. Read the questions carefully, I mix up p and q all the time


## [LOGIC SYMBOLS](https://en.wikipedia.org/wiki/Glossary_of_mathematical_symbols#:~:text=a%20category.-,Basic%20logic,-%5Bedit%5D)

### Conjunction ( ∧ )

- Logical AND
- p ^ q can translate to (x AND y) or (x && y)

### Disjunction ( ∨ )

- Logical OR
- Also known as Inclusive Or
- p v q can translate to (x OR y) or (x || y)

### Exclusive Or ( ⊻ )

- The way we normally use or in English. One or the other.
- You can go to Tim's class, or you can be a loser (jk)
- Also seen as ⊕

### Negation ( ¬ )
- Logical NOT
- Reverses the truth value of proposition
- If p is True then ¬p is False

**Order of Operations**
Parenthesis, Negate, AND, OR

### Truth Tables

Entries in a truth table have 2^n rows. Each column has equal number of true and false entries. We can see alternating patterns of T and F. The main way to fill out a truth table is to fill the first column split in half, top half with T's, bottom half with F's.

When evaluating compound propositions, we should evaluate individual expressions first. For instance NOT p AND (q OR r) can be broken down into an evaluation of NOT p as a unary expression, as well as the statement within parentheses as a binary expression. Not p has its own set of values, then the evaluation of q OR r yields its own set of values, and the results of those two distinct values can be evaluated as a final binary expression.
## Conditional Statements

A compound proposition that uses a conditional operation is called a **conditional proposition**, also known as a conditional statement.

### If Then ( → )
- p → q reads as if p then q
- proposition p is the hypothesis and proposition q is the conclusion
- 
- Evaluation of this proposition is true when p and q are both true, false if p is true but q is false.
- | p | q | p → q
  | --- | --- | --- | 
  | T | T | T |
  | T | F | T |
  | F | T | T |
  | F | F | T |
  
- Represents a contract. 
	- If p is true, then the contract breaks when q is false.
	- Doesn't have to be fair, only indicates a contract if p is fulfilled, then q HAS to be fulfilled. Says nothing about if p ISNT fulfilled.

### Converse 
- if q then p

### Contrapositive
- if not q then not p

### Inverse
- if not p then not q

### If and Only If ( ↔ ) Biconditional Operation
- What we might traditionally think of with conditional logic or contracts
- p if and only if q, shorthand p iff q
- | p | q | p ↔ q |
  | --- | --- | --- |
  | T | T | T |
  | T | F | F |
  | F | T | F | 
  | F | F | T |
- I will mow your law if and only if you pay me: Statement is true if the lawn is mowed and I get paid, also true that if I don't mow the lawn, I don't get paid. If mow the lawn and don't get paid, contract is broken, if I get paid, but don't mow the lawn, the contract is also broken.

### Conditional Precedence

If parentheses are not given, then logical operators get precedence over conditional operators. When in doubt, just use parens.

### Tautology, Contradiction, Equivalence

| p | not p (q) | p iff q |
| --- | --- | --- |
| T | F | F |
| F | T | F |

A Tautology means that all results are true, contradiction is all results are false. Equivalence is when two statements yield the same truth results.

### De Morgan's Laws

Logical equivalences that show how to distribute negation operations inside a parenthesized expression

1. NOT (p OR q) ≡ NOT p AND NOT q
2. NOT (p AND q) ≡ NOT p OR NOT q

## Topics
Take This Fish/Orders of Ignorance
- Logical Math
	- https://www.youtube.com/watch?v=BrDyDQYRUxM
		- [Law of Excluded Middle From Standford](https://web.stanford.edu/~bobonich/glances%20ahead/IV.excluded.middle.html#:~:text=That%27s%20why%20it%27s%20called%20the,be%20one%20or%20the%20other)
		- [Law of Excluded Middle](https://en.wikipedia.org/wiki/Law_of_excluded_middle)
		- [Laws of Thought](https://www.britannica.com/topic/laws-of-thought)
- Multi-state machines
	- https://www.youtube.com/watch?v=fXwSFhUVFmE
- Why use base 2?
	- see above
Go Over Exercises

### About me
- I'm 30
- Background, WV, SP-BR, BYU-I, UVU, etc.
- I play guitar, enjoyer of death metal. Fallujah, rivers of nihil, ulcerate, aegaeon, cynic, death
- I love sushi, but really any dishes with rice I usually go crazy for
- Slight anime nerd. Eva, HxH, Trigun, .hack, Akira, Ghost in the Shell, CSM, JJK, etc
- R6 Siege, Elden Ring
- Reading, movies, hobby collection
### Class Structure
- We'll have a class-topics thread in discord. This is where you all will post questions that you have or material you want to especially talk about in class.
- I don't really go over slides. We'll talk about relevant class material, and any side topics that you all want covered. 
- We can go over a few of the assignment questions in class, and work through them together. In effect, one of the days each week will have something that's partially like a lab. We'll cover as much material as we need to, and work on some of the more challenging questions together.

### Warnings
- I do not make the coursework. I am an adjunct, not a mentor. Let me repeat that, I don't make the coursework, or any of the material. I'm here to deliver it to you, help you understand it, and guide you through the work. Someone had the audacity to complain about the fact that I didn't create my own material when I explained that day 1 a few semesters ago. I'm also not in control of zybooks. If there are issues, it's an administrative issue that comes from zybooks or the department. All I can do to fix things is send emails and hope people respond quickly. So let it be written, that I don't make the material.
- If attendance gets too low, I will enforce an attendance policy. I hate basing grades off attendance, but the overall class experience diminishes greatly if people aren't coming to class. Class is better with you there. 

### Success
- Get your sleep. Seriously, this is probably the most important thing. Staying awake burning the midnight oil might feel like what you're supposed to do, and with how fast things go, you might have to stay up a bit. But seriously, get your 8 hours, make sure you're rested. Take mental breaks. Come back to it if it's not clicking. If it comes down to you not sleeping so that you can get your project in on time, let me know, get your rest, and I'll flex the date by a day.
- Read. The CS major is really a reading and writing major. While we generally write lots of programs in this major, more than anything, what you're doing is communication.
- Get used to drawing/writing. Honestly, the easiest way to grasp material in this class is often to draw things out and walk through problem steps on paper, whiteboard, onenote, whatever.
- Group up. We don't tolerate plagiarism. But we do love it when students get together, explain topics to each other, suggest strategies for approaching a problem, help each other succeed, and make friends. 
- Have fun. Realize that although this course will be challenging, this is a real meat and potatoes course. This is one of the true CS classes that you'll take, with topics that'll be useful to you whether you're building compilers, working with assemblers, or writing DSL's. Look ahead to the future, and get pumped for the cool stuff you'll learn!
- Get ahead of the work. Don't lose the basically free points that come from the reading. Get those in on time. Even if you need to skim ahead, get your PA points. It's the freest way to get points, which will potentially give you more wiggle room on the exams and projects. They can be the deciding factor between matriculation or not.
- Engage during class-time. I know it's tough sometimes to speak up, and sometimes there might be someone who appears to know a lot, so you don't want to embarrass yourself. It's really fine though, we're all in different places, and chances are, a lot of other people are wondering the same thing you are, and big chances are, someone may not even realize they have a question (very dangerous). So pipe up, ask questions, and be engaged. We'll have a lot better of a time if everyone has fun and talks during class!