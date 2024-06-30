# Creating-a-virtual-Environment
We use a module named virtualenv which is a tool to create virtual environments in Python, isolated from system environment Python.
virtualenv creates a folder that contains all the necessary executables to use the packages that a Python project would need

#Installing virtualenv
```
$ pip install virtualenv


#Test your installation:
$ virtualenv --version

#Create a new Virtual Environment
$ virtualenv my_env

```
After running this command, a directory named my_env will be created. This is the directory that contains all the necessary executables to use the packages that a Python project would need.
This is where Python packages will be installed. If you want to specify the Python interpreter of your choice, for example, Python 3, it can be done using the following command:
```$ virtualenv -p /usr/bin/python3 virtualenv_name```

Activating a Virtual Environment in Python
Now after creating a virtual environment, you need to activate it. Remember to activate the relevant virtual environment every time you work on the project. This can be done using the following command:

Activate a Virtual Environment on Windows
To activate virtual environment using windows command prompt change directory to your virtual env, Then use the below command```
$ cd <envname>
$ Scripts\activate ```
Note: source is a shell command designed for users running on Linux (or any Posix, but whatever, not Windows).

Activate a virtual environment on Linux
$ source virtualenv_name/bin/activate

Once the virtual environment is activated, the name of your virtual environment will appear on the left side of the terminal.
![image](https://github.com/the-faaz/Creating-a-virtual-Environment/assets/161277809/410ec6cb-c6ec-4cea-8e03-8550bf385118)
This will let you know that the virtual environment is currently active.

Installing Dependencies in Virtual Environment Python
In the image below, venv named virtual environment is active. Now you can install dependencies related to the project in this virtual environment.

For example, if you are using Django 1.9 for a project, you can install it like you install other packages.
The Django 1.9 package will be placed in virtualenv_name folder and will be isolated from the complete system.

Deactivate Python Virtual Environment
Once you are done with the work, you can deactivate the virtual environment by the following command:
(virtualenv_name)$ deactivate
![image](https://github.com/the-faaz/Creating-a-virtual-Environment/assets/161277809/a5247a05-3e9f-4b8c-bcb1-3a59f0f884ca)
Now you will be back to the system’s default Python installation.
