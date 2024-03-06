# Convert Python Project To Executable using cx_freeze
This is a template repository code for converting Python script to Windows executable using the cx_freeze library

# Command to install the library
<pre>pip install cx_Freeze</pre>

# Instructions
First, place the setup.py file in the same folder where your main Python file is. After that, Place the name of the Python file under the "executables" variable and include any additional files under the "options" variable. Then, set the process's name, add a description, and save the changes.<br>
Now, open the terminal in the folder and run this command<br>
<pre>python setup.py build</pre>
This will compile the program under the "build" folder.

# How to add a program icon
Change the executables line to this:
<pre>executables = [Executable("python_file_name.py", base=base, icon="favicon.ico")]</pre>
After that, add the same "favicon.ico" in the same line as "include_files" so that it is like
<pre>"include_files": ["favicon.ico"],</pre>
Make sure to keep the icon file within the same folder too. Then run the build command, and the program will include the program icon.
