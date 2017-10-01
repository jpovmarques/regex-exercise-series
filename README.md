# REGEX EXERCISE SERIES 
by Prof. Maltsev

##

### SERIES ONE
Write a regex pattern that:

>_"Find all the comment lines inside a Python file."_
>
>```
>re.findall(r"(?<!= ')(?<!=')(?<!= \")(?<!=\")(?<!= \"\"\")(?<!=\"\"\")(#.*)", file, re.MULTILINE)
>```
>
>>Finds a comment where none exists:
>>```
>>my_string = "#HashtagsAreCool" (passed)
>>```

>_"Find all the function names that have a typified return type inside a Python file."_
>
>```
>re.findall(r"def (.+?)\(.*\) -> .+:", file)
>```
>
>>Fails to find this function:
>>```
>>def my_func(
>>        arg1: str,
>>        arg2: str,
>>): -> None:
>>    print(arg1, arg2)
>>```

>_"Find all the docstrings inside a Python file."_
>
>```
>re.findall(r"(\"\"\"[\S\s]+?\"\"\")", file)
>```
>
>>Does not include the last character in this funtion's docstring, when it finds it:
>>```
>>def my_func():
>>    """Prints \"Hello, world!\""""
>>    print("Hello, world!")
>>```


_file_ - could be any Python file dumped into a string_

__*This series has been graded:*__

![Much to learn you still have.](https://media0.giphy.com/media/3ohuAxV0DfcLTxVh6w/giphy.gif "Much to learn you still have.")


