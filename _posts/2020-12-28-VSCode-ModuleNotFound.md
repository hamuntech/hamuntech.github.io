---
layout: post
title: VSCode Code Runner 'ModuleNotFoundError'
---
In case you receive an error similar to the one as depicted below in Visual Studio Code while trying to run Python code in a xxx.py file, using the "Run Code" button on the top right hand side of the code window, then please use following process to resolve the issue.

**Error**
<pre>
[Running] python -u "/Users/test.py"
Traceback (most recent call last):
  File "/Users/test.py", line 13, in <module>
    import tensorflow as tf
ModuleNotFoundError: No module named 'tensorflow'

[Done] exited with code=1 in 0.065 seconds 
</pre>

**Resolution**

First, make sure that the "Run Code" button looks like this:

![CodeRunnerButton]({{ site.url }}/images/assets/vscode_cr1.png "Code Runner Button")

Then, click on the Extensions option in the left side bar and search for "code runner". Select Code Runner and uninstall it. Once completed, come back to the code window and notice that the button to run code has changed to a green button, similar to the one below, and now you should be able to run Python code without any issues. 

![PythonRunButton]({{ site.url }}/images/assets/vscode_cr2.png "Run Python Code Button")

Note that this is not an issue with Visual Studio Code, but rather its related to the Code Runner extension. 

Happy Coding!
