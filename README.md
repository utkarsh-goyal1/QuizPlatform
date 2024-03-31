Create a Quiz----
->When the user clicks on create quiz button then "CreateQuiz" component will get display. It asks the user for quiz title and time.
->When the user clicks on add question button then a quiz code is generated and (quiz title, time, quiz code) will save on backend.After that "Questions" component will get display to add the question.
->When the "Questions" component will display then we will fetch the quiz from the backend on the basis of quiz code to display the quiz details for which we are adding questions.
->In "Questions" component there is a button to add a question . When the user clicks on that button then "NewQuestion" component will get display.When this component will get display then i will fetch the data of 
  quiz from the backend to find the question number.After filling the details of the question, when the user clicks on the save question button then i will call a api to save that question in db and save in the 
  questions array of that particular quiz.
->After that When a user clicks on the save quiz button then i will redirect the user to Home page because quiz has already been saved.

