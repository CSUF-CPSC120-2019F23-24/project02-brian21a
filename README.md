#  Project Milestone 2 Objectives
1. Learn to use C++ manipulators and the stringstream object
2. Output results in different forms
3. Compile and run program

# Business Trip Expenses
In this program, you will be learning to use the C++ programming data manipulators.

# Prerequesites
`main.cpp` from project milestone 1

## main.cpp
Update project milestone 1 in the following ways:
1. Allow multiple words for the business trip location
1. Add range checking to the business trip location *(hint: output no more than 20 characters, using `substr` from the `string` object)*
1. Add dollar signs to your output (see sample) *(hint: copy $ and dollar value to a string before outputting, example string would be $649.20)*
1. Update the dollar amounts so that they always show 2 digits past the decimal

The program then outputs all categories along with the total of all expenses in table format. See Sample Output below for format. *Note that information following the question marks in the sample output is user input, and not a part of your program.*

# Hints
1. Copy the dollar sign character and amount into a string before outputting it
1. Make sure you have set the field widths wide enough to allow all values to line up properly
1. Don't forget to add comments to explain what the code is doing
1. Choose variable names that explain the purpose of the variable

# Sample Output
```
Welcome to the Business Trip Tracker!

What is the business trip location? New York City
How many days will the trip take? 3
What is the total hotel expense? $649.2
What is the total meal expense? $220.8

Location         Days       Hotel       Meal       Total
New York City       3     $649.20    $220.80     $870.00
```

# Completion checklist
1. Did you comment your code where appropriate?
1. Did you use variable names appropriate for the purpose/usage of the variable?
1. Does your program compile? (i.e. no errors when you run clang++)
1. Does your program produce the desired results? *Hint: try changing the input values from those in the "Sample Output" to something very simple (such as $3.10 hotel expense and $4.30 meal expense) and verify that your program produces the correct "Total"*
1. **After checking in your program into git using the command line, please refresh the GitHub Website and click on your file to make sure your latest updates exist in the file on GitHub.**

# Project exercise guide
Here's a link to the [Project exercise guide](https://drive.google.com/open?id=1BbuqywMqBWSAIQjEn1RaBhSDZAbSknUw) in case you need to review the lab exercise objectives, grading scheme, or evaluation process.

# Code evaluation
Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of `/home/student/labex01-tuffy` and you are currently in `/home/student` you can issue the following commands

```
cd project01-tuffy
```

Use the `clang++` command to compile your code and the `./` command to run it. The sample code below shows how you would compile code saved in `main.cpp` into the executable file `main`. Make sure you use the correct filenames required in this problem.  Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

```
clang++ -std=c++17 main.cpp -o main
./main
```

# Submission
1. To upload your code into the GitHub repository, the first step is to add your code to what is called the staging area using git's `add` command. The parameter after `add` is the name of the file you want to add. There are cases when you have multiple changed files, so you can just type . (period) to add all modified files.

    ```
    git add .
    ```

1. Once everything is in the staging area, we use the `commit` command to tell git that we have added everything we need into the staging area. This command can be issued with a message informing users of the changes made.

    ```
    git commit -m "short description of code changes being uploaded"
    ```

1. In case it asks you  to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and GitHub username.

    ```
    git config --global user.email "tuffy@csu.fullerton.edu"
    git config --global user.name "Tuffy Titan"
    ```

    When you're done, make sure you type the `git commit` command again.

1. And finally, you can upload all changes to the GitHub repository using git's `push` command. Provide your GitHub username and password when you are prompted for these.

    ```
    git push
    ```

1. When you finish the exercise, go back to Titanium and click on the `Add submission` button in the lab exercise page. Provide a short message *that includes your GitHub username* in the text area such as "user tuffy - finished lab exercise" and click on `Save changes`. Finally, click on `Submit assignment` to inform your instructor that you are done.
