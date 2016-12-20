Sample Cython packaged project
===============================

Is recommended that you do this inside a virtualenv environment. Once in just
do

```
pip install -r requirements-dev.txt
```

and then

```
python setup.py bdist_wheel
```

This will create a build and a dist directory containing the compiled binary
and the packaged wheel file. You will find the wheel file inside the dist
directory named say_hello-0.1-cp27-cp27mu-linux_x86_64.whl or similar. The name
will depend on the architecture and python version you are using.

To install the file simply use pip

```
pip install dist/say_hello-0.1-cp27-cp27mu-linux_x86_64.whl
```

To test it out we can fire up the python interpreter

```
Python 2.7.12 (default, Nov 19 2016, 06:48:10) 
[GCC 5.4.0 20160609] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> import helloworld
>>> helloworld.say_hello('Python')
Hello Python
```





