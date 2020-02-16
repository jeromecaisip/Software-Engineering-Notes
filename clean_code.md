# Chapter 1 - Clean Code

1. Clean code looks like it was written by someone who cares.

2. As programmers, we are authors. It's an author's responsibility to for communicating well with their readers.

3. Be professional. Defend the codebase with passion, it's unprofessional for a programmer to bent to the will of the managers
who don't understand the risks of making messes.

4. Bad code is more expensive in the long run. In terms of providing value to the business, bad code decreases productivity over time because bad code leads to more bad codes,
and eventually will lead to abandonment of the codebase which is more expensive.

5. In software, 80% or more of the work is maintenance, so if you want to succeed you have to make the code
maintainable and clean. 

6. Good software requires discipline, presence of mind and thinking.

7. Total Productive Maintenance (TPM) pillars/5s:
    - Sort  - Throw away unused things. Remove legacy code, unused methods and variables, commented and duplicated code, etc.
    - Systematize - A piece of code should be where you expect to find it, if not re-factor to get it there.
    - Shine - Clean often (eg.remove old comments, unneeded code, refactor, write and run tests). Apply "Boy scout rule".
    - Standardize - Set a coding standard, quality checks, process, etc.
    - Sustain/Self-discipline - Adhere to the standards and always do the right thing.


8. Boy scout rule. (Leave the ground cleaner when you found it)


# Chapter 2 - Meaningful Names

1. Use intention revealing names.

2. Avoid disinformation. 

3. Make meaningful distinction. If names are different, then they should also mean something different.

4. Use pronounceable names.

5. Use searchable names.

7. Avoid encodings.

8. Avoid hungarian notation.

9. Avoid mental mapping.

10. Class names should have noun or noun phrase names.

11. Methods/functions should have verb or verb phrase names.

12. Pick one word per concept (avoid using synonymous words). (eg. fetch, get, retrieve) and (manager, controller, driver)

13. Don't pun. Don't use same word two two purposes.

14. Use solution domain names for code for code that has more to do with the CS/technical/programming  concepts.

15. Use problem/business domain names for code that has more to do with the problem/business domain concepts.

16. Add meaningful context when a name is not meaningful enough by themselves. (eg. prefixing)

17. Don't add unnecessary context.


# Chapter 3 - Functions

1. Functions should be small. 

2. Blocks and indenting. Block within `if`, `else` , `while` and so on should only be one/two line long. Probably that line should be a 
function call. Indent level should not be greater than one or two.

3. It should do one thing. They should do it well. They should do it only. 

4. Function that do one thing cannot be reasonably divided into sections.

5. One level of abstraction per function. (step down rule)

6. Use descriptive names. Be consistent with naming, should allow the sequence to tell a story.

7. Try to minimize function arguments. If the functions requires more than two to three arguments, probably they should be wrapped into a class or object.

8. Avoid [flag arguments](https://www.martinfowler.com/bliki/FlagArgument.html).

9. Have no side-effects. (It violates the rule: Do one thing well.)

10. Avoid output arguments. [Output arguments are objects that the method operates on, and then returns](https://medium.com/@webprolific/my-takeaways-from-clean-code-a70ca8382884). 
If your function must change the state of something, have it change the state of its owning object.

11. Command Query Separation. Function should either do something or answer something, but not both.

12. Prefer exceptions rather than error codes.

13. Extract the bodies of `try/catch` blocs out into functions of their own.

14. Functions should do one thing. Error handling is one thing. Thus, a function that handles errors should do nothing else. See no.13 .

15. DRY (Don't repeat yourself). Refactor to make things DRY.

16. "Make it work. Make it right. Make it fast.". Writing good functions is a process. Write a draft first then refactor while keeping the tests passing. 







