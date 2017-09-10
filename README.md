# REGEX EXERCISE SERIES 
by Prof. Maltsev

##

### SERIE ONE
Write a regex pattern that:

>_"Find all the comment lines inside a Python file."_
>
>```
>re.findall(r"(#.*)\n",file)

>_"Find all the function names that have a typified return type inside a Python file."_
>
>```
>re.findall(r"def (.+?)\(.*\) -> .+:", file)

>_"Find all the docstrings inside a Python file."_
>
>```
>re.findall(r"(\"\"\"[\S\s]+?\"\"\")", file)


_file_ - could be any Python file dumped into a string_

__*This series has not yet been corrected*__


