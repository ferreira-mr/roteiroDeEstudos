# Learning Python - Mark Lutz
#Estudos/DataScience/Python/Livros
[[Python]]

<a href='LearningPythonPowerfulObjectOrientedProgramming2013.pdf'>LearningPythonPowerfulObjectOrientedProgramming2013.pdf</a>

## Part I - Getting Started
### Chapter 01 - A Python Q&A Session
#### Test Your Knowledge: Quiz
	1. What are the six main reasons that people choose to use Python?
	2. Name four noble companies or organizations using Python today.
	3. Why might you not want to use Python in an application?
	4. What cay you do with Python?
	5. What’s the significance of the Python **import this** statement?
	6.  Why does “spam” show up in so many Python examples in books and on the Web?
- - - -
### Chapter 02 - How Python Runs Programs
#### Test Your Knowledge: Quiz
	1. What is the Python interpreter?
	2. What is source code?
	3. What is byte code?
	4. What is the PVM?
	5. Name two or more variations on Python’s standard execution model.
	6. How are Python, Jython, and Iron Python different?
	7. What are Stackless and PyPy?
- - - -
### Chapter 03 - How You Run Programs
#### Chapter Summary
In this chapter, we’ve looked	at common ways to launch Python programs: by running code typed interactively, and by running code stored in files wit system command lines file icon clicks, module imports, exec calls, and IDE GUIs such as IDLE. We’ve covered a lot of pragmatic startup territory here. This chapter’s goal was to equip you with enough information to enable you to star writing some code, which you’ll do in the next part of the book. There, we will start exploring the Python language itself, beginning with its core data types — the objects that ares the subjects of your programs. 
First, though, take the usual chapter quiz to exercise what you’ve learned here. Because this is the last chapter in this part of the book, it’s followed with a set of more complete of programs, or just for a refresher, be sure to turn to Appendix D after you’ve give the exerciser a try.

#### Test Your Knowledge: Quiz
	1. How can you start an interactive interpretar session?
	2. Where do you type a system command line to latch a scrip file?
	3. Name four or more was to run the code saved in a script file.
	4. Name two pitfalls related to clicking file icon on Windows.
	5. Why might you need to reload a module?
	6. How do you run a scrip from within IDLE ?
	7. Name two pitfalls related to using IDLE.
	8. What is a namespace, and how does it relate to module files?
- - - -
## Part II - Types and Operations 
### Chapter 04 - Introducing Python Objects Type
#### The Python Conceptual Hierarchy
::**PROGRAMS** are composed of **MODULES**::
::**MODULES** contain **STATEMENTS**.:: 
::**STATEMENTS** contain **EXPRESSIONS**::
::**EXPRESSIONS** create and **PROCESS OBJECTS**::

#### Why Use Built-in Types?
Here are some reason why:
	- Built-in objects make programs easy to write.
	- Built-in objects are components of extensions.
	- Built-in objects are often more efficient than custom data structures.
	- Built-in objects area a start part of the language.

#### Operation with sets

```python
X = set('span')
Y = {'p', 'm', 'a', 's'}

X & Y # Intersect
X | Y # Union
X - Y # Diference
X > Y # Superset
```

- - - -
### Chapter 05 - Numeric Types

#### Chapter Summary
This chapter has taken  a tour of Python’s numeric objets types and the operations we can apply to them. Along the way, we meant the standard inter and floating-point types, as well as some more exotic and less commonly used types such as couples number, decimals, fractions, and sets. We also explored Pythons’s expression syntax, type conversion, bitwise operations and various literal form for coding mounters in scripts .
Later in this part of the book, we’ll continue our in-depth type tour bi filling in some details about the next object type-the string. In the next chapter, however, we’ll take some time to explore the mecânica of variable assignment in more detail than we have here. This turns out to be perhaps the most fundamenta idea in Python , so make sure you Che out the next chapter before moving on. First, though, it’s time no take the usual chapter quiz.
- - - -
### Chapter 06 - The Dynamic Typing Interlude

#### Chapter Summary
This chapter took a deeper look at Python’s dynamic typing model - that is, the way that Python keeps track of object types for us automatically, taster than requiring us to code declaration statements in our scripting. Along the way, we learned how variables and objects are associated by references in Python; we also explored the idea of garbage collation, learned how shared references to objects ca affect multiple variables, and saw how references impact he notation of equality in Python.
Because here is  one assignment model in Python, and because assignment pops up everywhere in the language, it’s important that you have a handles on the model before moving on. The following quiz should help you review ops of this chapter’s ideas . After that ,we’ll resume to core objects tou in the next chapter, with strings.

#### Test Your Knowledge: Quiz
1. Consider the following three statements. Do they change the value printed for **A**?
```python
	A = 'span'
	B = A
	B = 'shrubbery'
```

2. Consider the three statements. Do they change the printed value of **A**?
```python
	A = ['span']
	B = A
	B[0] = 'strubbery'
``` 

3. How about these - is **A** changed now?
```python
	A = ['span']
	B = A[:]
	B[0] = 'strubbery'
``` 

#### These Your Knowledge: Answers
1. No: A still prints a “span”. When **B** is assigned to the string **”shrubbery**, all that happens in that the variable **B** is reset to point to the new string object. **A** end **B** initially share (I.e., reference/point) the same sing string object **”spam”**, but two name are never lined together in Python. Thus, setting **B** to a different object has no effect on **A**. The same would be true if the last statement here were **B = B + “shrubbery”**, the way - the concatenation would make a new object for ties result, which would then be assigned to **B** only. We can never overwrite a string (or number, or tule) in place, because string are immutable.

3. Yes: **A** now pints as **[“shrubbery”]**. Technically, we haven’t really changed either **A** of **B**; instead, we’ve changed part of the object hey both reference (point to) by overwriting that object in place thorough the variable **B**. Because **A** referes the same object as **B**,  the update is reflected in **A** as well. 
4. No: A still prints as **[’span’]**. The in-place assignment through **B** has no effect this time because the slice expression made a copy of the list object before it was assigned to **B**. After the second assignment statement, there are two different list objects that have the same value (in Python, we say hey are ==, bu not is). The third statement change the value of the list object pointed to by **B**, but not that pointed to by **A** .

### Chapter 07 - String Fundamentals

#### Chapter Summary
In this chapter, retook an in-depth tour of the string objects type. We learned about coding string literals, and we explored string operations, including	sequence expression,  stings method calls, and string formatting with both expressing and method calls. Along the way, we studied a variant of concepts in depth, such as slicing, method  call syntax, and triple-quoted block string. We also defined some core ideas common to a variety of types: sequences, for example, star an entire set of operations.

```python
reply = """
Greeting...
Helo %(name)
Your age is %(ages)s
"""

values = {'name' : 'Bob', 'age': 40}

print(reply % values)

food = 'spam'
qty = 10
vars()

print('%(qty)d mode %(food)' % vars())
```

#### Test Your Knowledge: Quiz
1. Can the string **find** method be used to search a list?
2. Can a string slice expression be used on a list?
3. How would you convert a character to its ASCII integer code? How would you convert the other way, from an interference to a character?
4. How might you go about changing a string in Python?
5. Give a string **S** with the value **’s,pa,m’**, name two ways to extract the two characters in the middle.
6. How many characters are there in the string **“a\nb\x1f\ood**?
7. Why might you use the **string** module instead of string meths calls”

#### Test Your Knowledge: Answers
1. No, because methods area allies types-specific; that is, the only work on a single data type. Expression like **X+Y** and built-in functions like **len(X)** are generic, though  and  may work on a variety of types. In this case for instance, the **in** membership expression has a simile effect as the string find, but it can be used to search both string and list. In Python 3, there is some attempt to gore meths by categories (for example, the mutable sequin types **list** and **bytearray** have similar method sets), but methods, expression are generic and apply too many types-specific the other operation sets.
2. Yes. Unlike methods, expression are genes and applicable too many types, In this case, te slice expression is real a sequence operation - it works on any type of sequence object, including string , list , and tuples. The only difference is that queen you slice a list, you get back a new list.
3. The building-in **ord(S)** function converts from a one-character string to an integer caracter code; **chr(I)** converts from the integer code back to a string. Keep in mind, though, that these interred are only ASCII codes for text whose characters are drawn only from ASCII caracteres set. In the Unicode model, text string are really sequences of Unicode code point identifying integers, which may fall outside the 7-bit range of number research by ASCII.
4. String cannot be changed; they are immutable . However, you can achieve a similar effect by creating a new string — by concatenating, slicing , ruining formatting expression. Or using a method call like **replace** and then assigning the result bak to the original variable name.
5. You can slice the sting suing **S[2:4]**, or split on the comma snd indeed the string using **S.split(‘,’)[1]**. Try theses interactively to see for yourself.
6. Six. The string  **“a\nb\x1f\ood** contains the characters **a**, new line (**\b**),  **b**, binary **31**(a hex scape \**x1f**), binary 0 (an octal escape **\000**), and **d**. Pass the string to the buit-in- **len** function to verify this, and print each of its caracter’s **ord** result to see the actual code point (indentifying number) value. 
7. You should never user the **string** module instead of string object mahouts call today — it’s deprecates, and its calll are removed completely in Python 3. The only valid reason for using the **string** module at all today is for its other tools, such as predefined constants. You might also see it appears in what is now vey old and dusty Python code (and books of the misty past — like 1990s).

### Chapter 08 - Lists and Dictionaries

#### Chapter Summary
In this chapter, we explored the list and dictionary types — probably the two most common, flexible and powerful collection types you will see and use in Python code. We learned that the list type supports positionally orders collections of arbitrary objects, and that may freely nested and grown and shrunk on demand. The dictionary the is similar, but it stores items by key instead of by position and Dows no maintain any reliable left-to-right order among its item. Both list and dictionaries are mutable and so support a variety of in-place change operations not available for string: for example, list can be grown by append calls, and dictionaries by assignment to new keys.
In the next chapter, we will wear up our in-depth core objet type tour by looking at tuple and files. After that, we’ll move on to statements that code the logic that  processes our objects, taking us another step toward writing complete programs. Before we tackle those topics, though, here are some chapter quis question review.

#### Test Your Knowledge: Quiz
1. Name two ways to build a list containing five integer zeros.
2. Name two ways to build a dictionary with two keys, ‘a’ and ‘b’, each having and associated value of 0.
3. Name four operation that change a list object in place.
4. Name for operation that change a dictionary object in place.
5. Why might you use a dictionary instead of a list?

#### Test You Knowledge: Answers
1. A literal expression line` [0, 0, 0, 0]` and a repletion expression like `[0] * 5` will each create a list of five zeros In practice , you might also build one up a loop that tart with an empty list na appends ) to it in each iteration, with `L.append(0)`. A list comprehension `[0 for i in range(5)] `could work here, too, but this more work than you need to do for this answer.
2. A literal expression such as `{‘a’  :  0,  ‘b’ : 0}`  or a series of assignments like `D = {}, D[‘a’] = 0, D[‘b’] = 0` would create the seared dictionary . You can also use the newer and simpler-to-code dict(a=0, b=0) keyword from, or the more flexure `dict([(‘a’, 0), (‘b’, 0)])` key/value sequences form. Or, because all the values are the same, you can use the special from `dict.fromkeys(‘ab’ 0)`. In 3.X and 2.7, you can also use a dictionary comprehension: `{k : 0 for k in 'ab'}`, though again, this may be overkill here.
3. The **append** and **extend** methods grow a list in place, the **sort** and **reverse** methods order and reverse lists, the **insert** meths inserts an item at an offset, the **remove** and **pop** methods delete from a list by value and by position the **del** statement deletes an mite or slice, and index and slice assignment statements replace an item or entire section. Pick any four of these for the quiz.
4. Dictionaries are primarily changed by assignment to a new or existing key which creates or changes the key’s entry in the table. Also, the **del** statement deletes a key’s entry, the dictionary **update** method merges one dictionary **update** method merges one dictionary into another in place, and **D.pop(key)** removes a key and returns the value in had. Dictionaries also have other, more exotic in place change methods no present in this chapter, such as **setdefault**; see reference sources for more details.
5. Dictionaries are generally better the data is labeled (a record with files names, for example); list are best suited to collections of unlabelled items (such as all the files in a directory). Dictionary lookup is also usually quicker than searching a list, though this might very per program.

### Chapter 09 - Tuples, Files, and Everything Else.

#### Chapter Summary
This chapter explored the lat two major core object types — the tuple and the file. We leaned that tuples support all the usual  sequence operations, have just few methods, do no all any in-place changes because they are immutable, and are exited by the maned tuple type. We also learned by the build-in **open** function and provide methods for reading and writing data.
Along the way we explored how to translate Python objects to and from strings for storing in files, and we look at the **pickle**, **json**, and **struct** modules for advanced roles (object serialisation and binary data). Finally, we wrapped up by reviewing some properties common to all object types (e. g., shared references) and went through a list of common mistakes (“gotchas”) in the object type domain. 
In the next part of this book, we’ll shift gears, turning to the topic of *statement syntax* — the way you code processing glory in your scripts. Along the way, this next part expires an introduction to PYthon’s general syntax models which is applicable to all statement types. Before moving on, though take the chapter quiz, and then work though the end-of-part lab exercises to review type concepts. Statements largely just create and process objects, so make sure you’ve mastered this domain by working thoughtcrimes all the exercises before reading on.

#### Test Your Knowledge: Quiz
1. How can you determine how large a tuple is? Why is this tools locate here it is?
2. Write an expression that change the first item in a tuple. (4, 5, 6) should become (1, 5, 6) in the process.
3. What is the default for the processing mode argument in a file *open* call?
4. What module might ou use to store Python objects in a file without converting them to string yourself?
5. How might you go about coping all parts of a nested structure at once?
6. Who does Python consider an object true?
7. What is your quest?

#### Test Your Knowledge: Answers
1. The build-in **len** function return the length (number of contained items) for any container object in Python, including tuples. It is a built-in instead of a type method because it applies to may different types of objects. In genera, built-in function and expression may span any object types; method are specified to a single object type, though some may be available on more than one type (index, for example ,wore on lists and tuples).
2. Because they are immutable, you can’t really change tuples in place, but you can generate a new tuple with the seared value. Give `T = (4, 5, 6)`, you can change the first item by making a new tuple from tis parts by slicing and concatenating: `T = (1,) + T[1:]`. (Recall that a single- item tuples requires a trailing comma.) You could also convert the tuple to a lis, change it in place, and covert it back to a tuple, but his is more expensive and is rarely required in practice — simply use a list if you know that the objet will require in-place change.
3. The default for the procession mode argument in a file **open** call is ‘r’, for reading text input. For input tex files, simple pass in the external file’s name.
4. The **pickle** module can be used to store Python objects in a file whiteout explicitly converting them to strings. The **structs** module is relates, but it assume the data is be in packeting binary format in the file; **json** similarly coverts a limits set of Python objects to and from strings per the JSON format.
5. Import the **copy** module, and call **copy.deepcopy(X)** if you need to copy all part os a nested structure X. This is also rarely seen in practice; references are usually the desired behaviour, and shallow copies (e.g., **aList[:]**, **aDict.copy()**,  **set(aSet)** usually suffice for most copies.
6. An object is considered true if is either a nonzero number or nonempty collections object. The built-in world **True** and **False** are essentially predefines to the same meaning as integer **1** and **0**, respectively.
7. Acceptable answers include “To learn Python”,  “To move on the next part of the book”, or “The seek the Holy Grail.”

~~#### Test Your Knowledge: Part II Exercises~~
~~This session asks you to get your feet wet with built-in objects fundamentals. As before a few new ideas nat pop up along the way, so be sure to flip to the answers in appendix D when you’re done (os even when you’re not). If you have limited time, I suggest starting with exercises 10 an 11 (the most practical of the bunch), and then working from first to last as time allows, This all fundaments material, so try to do as many of these as you can; programming is a hands-on activity, and there is no substitute for practicing what you’ve read to amen ideas gel.~~

~~1. *The basics*. Experiment interactively with the common type operations found in the various operation tables in this part of the book. To get started, bring up the Python interactive interpreter type each of the following expression, and try to explain that’s happing in each of case. Note that the semicolon in some of these is being used as a statement separator, to squeeze multiple statements onto a single line: for example, **x = ; x** assigns and them print a variable (more on statement syntax in the next part of the book). Also remember that a comma between expressions usually builds a tuple, even there are no enclosing parentheses: X, Y, Z is a threes-item tuple, which Python prints back to you in parentheses.~~

## Part III - Statements and Syntax

### Chapter 10 - Introducing Python Statements

#### Chapter Summary
That concludes out quick loop at Python statement syntax. This chapter introduced the general rules for coding statements and cloys of code.  As you’ve leaned, in Python we normally code one statement per line and indent all the statements in a nested block the same amount (indentations is part of Python’s syntax). However, we  also looked at a few exceptions to these rules, including continuation lines and sing-le tests and loops. Finally, we put these ideas to work in an interactive script that demonstrated a handful of statements and showed statements synth in action.
In the next chapter, we’ll start to dig, deeper by going over each of Python’s basic procedure statements in dept. As you’ll see, thought, al statements follow the same general rules introduced here.

#### Test Your Knowledge: Quiz
	1. What three sign are require in a C-like language but committed in Phython?
	2. How is a statement normally termites in Python?
	3. How are the statements in a nest block of code normally associated in Python?
	4. How can you make a single statement span multiple lines?
	5. How can you code a compound statement on a single line?
	6. Is there any valid reason to types a semicolon path the end of a statement in Python?
	7. What is a **try** statement for?
	8. What is the most common coding mistake among Python beginners?
	
#### Test Your Knowledge: Answers
	1. C-like languages requires parentheses around the tests in some statement, semi-colons at the end of each statement, and braces around a nested block of code.
	2. The end of a line  terminates the statement that appears on that line. Alternatively, if more than one statute appears on the same line ,this can be terminated with semicolons, similarly, if a statement span Manu line, you must terminate it by closing a bracket syntactic pair.
	3. The statement in a nested block are all indented the same number of tabes or spaces.
	4. You can make a statements span many line by enclosing part of it in parentheses, square brackets, or curly braces; the statement ends when Python sees a line that contains the closing part of the pair.
	5. The body of a compound statement can be moves to the header line after the colon, but only if the body consists of only non compound statements.
	6. Only when you need to squeeze more than one statement onto a sing line of code. Even then, this only works if all the statement are non compound, and it’s discourage because it can lead to code that is difficult to read.
	7. The **try** statements is used to catch and recovery from exceptions (error) in a Python script. It’s usually an alternative to manually checking for errors in your code.
	8. Forgetting to type the colon charter at the end of the header line in a compound statement is the most common beginner’s mistake. If you’re new to Python and haven’t made it yet, you probably will soon!

### Chapter 11 - Assignments, Expression, and Prints

#### Chapter Summary
In this chapter, we began our in-depth look at Python statements by exploring assignments, expressions, and print operations. Although these are generally sync to use, they have some alternative form that, while optional, are often convenient in practice — augmented assignment statements and the redirection form of print operation, for example, all us to avoid some manual coding works. Along the way, we also studied the syntax of variables names, stream redirection techniques, and a piety of common mistake to avoid, such as assigning the result of an **append** method call back to a variable.
In the next chapter, we’ll continue our statements tour by filling in detail about the **if** statement, Python’s main selection tools; there , we’ll also revisit Python’s syntax model in more depth and look at he at the behaviour of Boolean expression. Before we move on, though, the end-of-chapter quiz will test your knowledge of what you’ve learned here.

#### Text Your Knowledge: Quiz
	1. Name three ways that you can assign three, variables to the same value.
	2. Why might you need to care when assigning three variables to a mixable object?
	3. What’s wrong with saying `L = L.sort()`?
	4. How might you use the **print** operation to sed Texto to an external file?

#### Text Your Knowledge: Answers
	1. Your can use multiple-target assigments `A = B = C = 0`, sequence assignment ( `A, B, C = 0, 0, 0`, or multiple assignment statements on three separate lines `A = 0, B = 0 and C = 0`. With the latter technique, as introduced in Chapter 10, you can also string the three separes statements together on the same line by separating them with semicolons `A = 0; B = 0; C = 0`.
	2. If you tem this way:`A = B = C = []` all the three names reference the same object, so changing it in place from one (e.g., **A.append(99)) will affect the other. Tis is true only for in-place changes to mutable objects like lists and dictionaries; for immutable objects such as numbers and string, this issues is irrelevant.
	3. The list sort meths is like **append** in that it makes an in-place assignment back to L sets L to None, not to sorted list. As discussed both earlier and later in this book (e.g., Chapter 8), a newer built-in function, **sorted**, sorts any sequence and returns a new list with the sorting result; because this is not an in-place change, its result can be meaningfully assigned to a name.
	4. To print to a file for a single **print** operation, you can use 3.X’s `print(X, File=F) `call from, use 2.X’s extend `print >> file`, X statement form, or assign `sys.stdou`to a manually opened file before the `print`and restore the origina after. You can also redirect all of a program’s printed text to a file with special syntax in the system shell, but this is outside Python’s scope.

### Chapter 12 - if  Test and Syntax Rules

> Switch Case pythonic  
```python
Choice = ‘ham’

branch = {'spam' : 1.25, 'ham'= 1.99, 'eggs' =  0.99}

print(branch['choice'])

>>> print(branch.get('spam' , Bad choice'))
1.25

>>> print(branch.get('bacon' , 'Bad choice')) # Use this feature with functions
Bad choice
```

#### Chapter Summary
In this chapter, we studied the Pytho **if** statement. Additionally, because this was our first compound and logical statement, we reviewed Python's  general syntax rules and explored the operation of truth values and test in more dept than we were able to previously.  A lent the way, we aso looked at how to code multiway branching in Python, learned about the  **if/else** expression introduced in Python 2.5, and explored some common ways that Boolean value crop up in code.

#### Text Your Knowledge: Quiz
	1. How might you code a multiway branh in Python?
	2. 
