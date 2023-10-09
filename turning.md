## Lab Report 1

---
# Change Directory

1. Running command with *no* arguement
we are currently in the **home** directory.
Having *no* arguements meant that there was no change or output from the terminal.
We are currently still in the **home** directory as seen in the picture below.

![Image](cd_no_arg.png)

2. Running command with a *path to a directory* as an arguement
We are currently in the **home** directory.
We imput this:

''' 
cd /home/lecture1/messages/
'''
we see that the present working directory *(pwd)* is messages rather than home.
This is not an error rather a **correct** way to change directory.

*view picture below*

![Image](cd_filepath.png)


3. Share an example of using the command with a path to a **file** as an arguement.
We are starting from the home directory again.
This time we are going to the *file en-us.txt*
We can an error in this instance, due to the fact that we are going to a **File** rather than a **Directory**.
Change directory can only switch to directories and in this case we are trying to change to a txt file.

![Image](cd_tofile.png)

---


# List

1. Running command with *no* arguement

If we are currently in lecture1 directory, if we run ls it lists all the **files and other directories** that are **directly under** the *current* directory in the unix file hierarchy. In the listing it highlights directories in blue. This is not an error
* doesnt change the directory you are currently in

![Image](LS1.png)

2. Path to a directory as an argument
We are currently in the **home** directory. When we run ls with a path to a directory it lists file's and other directories under the directory the path goes to. It doesnt cause an error, but rather a good way to see what is in directories other than what is the current.

![Image](LS_dir_path.png)

3. Path to a File as an arguement
The working directory was and even after running the code remains **home**.
The output is the path to the file, so it doesn't  list anything rather returns the path we input.
It is not an error, but since its not a directory, there are no other directories or files to return.

![Image]()







