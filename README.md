![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

Welcome tlamidi,

This is the Code Institute student template for deploying your third portfolio project, the Python command-line project. The last update to this file was: **August 17, 2021**

## Reminders

* Your code must be placed in the `run.py` file
* Your dependencies must be placed in the `requirements.txt` file
* Do not edit any of the other files or your code may not deploy properly

## Creating the Heroku app

When you create the app, you will need to add two buildpacks from the _Settings_ tab. The ordering is as follows:

1. `heroku/python`
2. `heroku/nodejs`

You must then create a _Config Var_ called `PORT`. Set this to `8000`

If you have credentials, such as in the Love Sandwiches project, you must create another _Config Var_ called `CREDS` and paste the JSON into the value field.

Connect your GitHub repository and deploy as normal.

## Constraints

The deployment terminal is set to 80 columns by 24 rows. That means that each line of text needs to be 80 characters or less otherwise it will be wrapped onto a second line.

-----
Happy coding!



In this project, it is about building a Simple Multiple choice Quiz using Python programing language. In actual fact , this is a small size project, but it could be used as a template for a bigger or different sizes of Multiple choice quize. This project targets wider range of different establishments in the society, groups, or possibly individuals, that would require some sort of quize or aptitude test to carry out an objective. Basically, Multiple choice quize is used primarily to test people's IQ, mental ability, choosing participant as been the best for a purpose, like in admission, employment, scholarship, entry level to participate in an occasion and in a competion between groups of people.  As a matter of fact, this project is intended for the society at large in the area of testing ability and selection for best or better candidate. 

The project in particular targets, some government departments to test people for different administrative reasons, for an example, driving test theory. Some are set up to test individual knowledge on different issues, including, academic subjects, planet, environment, current affairs, and many more. I title my Project "Simple Multiple Choice Quiz". 

I started the project by setting up Multiple choice Quiz, actually in a small size but could be added to as the case maybe. The whole idea is that, users would be asked to take a quiz, and at the end we keep track of the scores and then be able to tell the user how they did. In the project, I used some core codes in python, including classes, if statement, for loops and defined some functions.

The first thing is to represent the question and the test. There is a question prompt rolled out. Basically, there are two parts to this, there is a prompt, in other words the question itself, and also the answers to the questions. Both of these attributes needs to be tracked. What to asked and what the answer is. Inside the main file, I created a question class. The class will be able to store question prompt , and as well be able to store the question answer. For this purpose, I created another file, and I named it Question.py. I created a class inside the new file called, 'class Question'. Inside the class Question, I defined and initialised a function def__init__(self, prompt, answer): This function included the 2 attributes as the parameters, namely , prompt , and answer,The 2 values are assigned to actual class object, i.e,
'self.prompt = prompt, and self.answer = answer'. This complete equation class set up.

Inside the main file, next, was to creat a question object. Before this, in line 1 of the file , it should include a statement, that is, 'from Question import Question'. This is to import the question class. The question object created for each question, included  question_prompt with associated index, and answer. The format as shown, associated with a square bracket,
question = [
    Question(question_prompts[0], 'a')
    . . .
]

Next, is to write a function, that would run the test. It would confirm if the answer given by the user is right.
A parameter 'question' is passed into the function, ' def_run_test(questions)'. This represents the list of question object to ask the user. Within the function, there is a loop through all the question. The loop is through each question, and asked it to the user and get the user answer, and check to see if it is right. Within same loop, the operation also track how the user does through the test. Next line after the function statement, i created a variable called 'Score' and set it equal to zero. 
score = 0
Everytime the user gets it right,it will increment the score variable by one, i.e  'score += 1'
I loop through all the question in the question array. First created a 'for loop i.e 'for question in questions:
Basically, this is to ask user question and store the response inside the variable 'answer = input(question.prompt)'.
With 'if statement', this is to determine if the user get the question right. Giving, 'if answer == question.answer', this is to check if the answer the student gave is equal to the answer of the current question that were asking.If it is true, I just want to see score increment. That is score += 1. Basically we are adding 1 to the score.

Finally, within the loop, I would like to print the result. That is, to print out how many questions out of the total questions the user get right. Looking into the print statement,
        print("You got" + str(score) + "/" + str(len(questions)) + "correct") 
In the statement, 'Score' is the number of question user got right. With "str(score)", this is to first convert number into string. Also with str(len(questions,)), this is to first convert number into string, len() also to figure out how many questions were in the question array.
With the print statement, it would print out how many questions user got right.
Lastly the run_test function() is called. i.e
                run_test(questions).
