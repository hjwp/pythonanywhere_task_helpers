I want to check out the PythonAnywhere Education features
=========================================================

glyphicons_074_cup@2x.png

----

**Welcome to PythonAnywhere!**  Up here you will see instructions
walking you through the key features of our Education beta.

----

(If after closing this helper, you want to go through it again -- or try another
one -- go to the [Help page](/wiki/))

----


This page is your **Dashboard** -- your students will have one just like it.

Right now, we're on the **Consoles** tab, from which you
can launch interactive Python consoles, as well as a special type of console
called a **Bash** console, which is PythonAnywhere's main command-line console.
Try that now.

----

In your Bash console, type:

    python3.4
    >>> print("Hello world")

You'll see Python works the way you expect it to. Press Ctrl+D to exit.

----

Consoles are all very well, but often we want to save code to a file
using a text editor.  PythonAnywhere has a Python-specific text editor
built in.  Let's go check it out now.

Go back to the Dashboard by clicking the PythonAnywhere logo above, then
click through to the **Files** tab.

Type *hello.py* into the input box that says "enter a new file name",
and hit Enter.

----

That should have opened up a text editor. Let's try using it to
write some more Python code

    from datetime import datetime
    print("Hello, the time is {}".format(datetime.now()))


You can save your file, and if you wanted to you could go back
to a Bash console and run it from the command-line with 
`python3 hello.py`.  But there's a shortcut right on this
page -- click the "Save and Run" button (the black one with the three python
chevrons, **>>>**)

> (you may need to hit "allow popups" in your browser, then try a second time
> to see the new console appear)

----

So far, those were all basic PythonAnywhere features that any
user would get.  Now it's time to check out some of the Education-specific
features.

For this you'll need to open up a new "Private browsing" session in your web
browser, because we're going to create a "fake" student account, and set you
up to be its teacher.

You'll need to jump between this window and the private browsing session, to
continue following these instructions

----

In the private browsing tab, sign up for a second PythonAnywhere account.  You
can use the same email address as your main account if you like.

Once the account has been created, click through to its **Account** page, and
find the **Teacher** tab.  Enter your main account's username into this field,
and hit enter.

----

Then, still pretending to be a student in the private browsing window (hee hee),
go to the Files tab and start a new python file called
**studenthello.py**, with some simple code in it -- 

    print("Hello from student")

And hit the run button.

----

Now, back in your main account, hit **refresh** in your browser.

You should see a line at the top right of your dashboard, telling you
that you're logged in as you, and offering you a drop-down which will
let you switch to viewing your students' pages.

Use it now to click through to your students' dashboard. From there you'll be
able to see all their pages.  Try clicking through to their console, and you'll
see you can even type into it!

Notice that the little drop-down on your dashboard updates to tell you that you're
now viewing one of your students' pages.

You can return to your own dashboard by clicking your own username, or the main
PythonAnywhere logo.

----

Try typing something into the student's console, and then alt-tabbing across to
the private browsing session, and seeing it appear in their console.

----

You can also browse your students' Files tab, and all the other tabs.  

> Note that, while console sessions update dynamically, file editor sessions
> do not -- you can't see what the other person is typing, and you have to
> manually hit "refresh" if you want to see updates.


But there's a better way to interact with your students' files -- they are 
directly mounted into your own files area.

In your teacher account, go back to your Bash console, or open a new one
if necessary. Type `ls /home`, and you should see your own username, and your
student's username.

    >>> # press ctrl-d if you're still in a Python prompt

    $ ls /home
    myusername  mystudentusername

    $ ls /home/mystudentusername
    README.txt  studenthello.py

----

Let's imagine we want to create a programming assignment, and distribute
it to your students.  In the teacher account, go to the Files menu, and
create a new file called *week3_assignment.py*.  Give it the following 
contents:


    def add(number1, number2):
        # what should this function return?
        pass

    def say_hello(name):
        # adjust the next step so that, if someone calls the function with "Xerxes", the function prints "Hello, Xerxes"
        message = "?"  
        print(message)

Hit save, and go back to your Bash console.  Type this command:

    cp /home/myusername/week3_assignment.py /home/mystudentusername

And now your student has a copy of the assignment!

You can verify that in the private browsing session, or by clicking
through to them via the little dropdown in the top-right.

----

You can use the fact that you have full access to your students accounts to
distribute and later collect assignments, to help students to exchange code
with each other, and no doubt all sorts of other stuff that we haven't 
anticipated.

Go check out [the wiki](https://help.pythonanywhere.com/pages/Education) for more information, and be sure
to send us feedback and suggestions for improvements and new features!  We'd
love to hear from you.

[support@pythonanywhere.com](mailto:support@pythonanywhere.com)


