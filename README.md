# Linux-Bash-Issues
# My Linux terminal just malfuntioned and is printing out out previous errors to every command I add.

# Had Initially coded this:
import re

myString ='Send an email from this@email.com to test@user.com 34 times.'

result = re.search('Send', myString)

print(result)  

# The result I got was:
Original exception was:
Traceback (most recent call last):
  File "pw.py", line 8, in <module>
    import sys, pyperclip
  File "/usr/local/lib/python3.6/dist-packages/pyperclip/__init__.py", line 51, in <module>
    import platform
  File "/usr/lib/python3.6/platform.py", line 116, in <module>
    import sys, os, re, subprocess
  File "/home/andy/Desktop/Works_py/re.py", line 5, in <module>
    result = re.findall('^Send', myString)
AttributeError: module 're' has no attribute 'findall'
  
  # This goes on with every script I try to run in the bash - same error msg
  # What could be the problem?
  
