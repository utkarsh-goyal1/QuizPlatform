Create a Quiz----
->When the user clicks on create quiz button then "CreateQuiz" component will get display. It asks the user for quiz title and time.
->When the user clicks on add question button then a quiz code is generated and (quiz title, time, quiz code) will save on backend.After that "Questions" component will get display to add the question.
->When the "Questions" component will display then we will fetch the quiz from the backend on the basis of quiz code to display the quiz details for which we are adding questions.
->In "Questions" component there is a button to add a question . When the user clicks on that button then "NewQuestion" component will get display.When this component will get display then i will fetch the data of 
  quiz from the backend to find the question number.After filling the details of the question, when the user clicks on the save question button then i will call a api to save that question in db and save in the 
  questions array of that particular quiz.
->After that When a user clicks on the save quiz button then i will redirect the user to Home page because quiz has already been saved.

Join Quiz----
->When the user clicks on the join quiz button then i will fetch the data of the quiz using quiz code from the backend and navigate to "Quiz Display" Component.
->Now in "Quiz Display" component i will fetch the data of that quiz from the backend using the quiz id.Now Quiz contains an array of question ids . Now i will call an api to fetch questions of those question ids.
->Now set the quiz data and questions using useState hook.
->Now start the timer and display the first question of the quiz.
->Now when user clicks on the next button to get the next question then first of all i will update the score of the user by his answer of the previous question and will display the next question iteratively until
  all the question completed.
->When all the questions get completed then i will show a "Quiz Result" component to the user.When the user clicks on the save button then a function "updateQuizResult" will be called  which will call an api to 
 save the quiz result in the backend.Along with this i will also add the quiz,quizResult to quizPlayed,quizResult fields of the user at the backend.
->After this user will navigate to the Home Page.

Checking Quizzes Created-----
->When the user clicks on the created(Quizzed Created) button then "CreatedQuizzez" component(in Cards folder) will get display and will fetch all the quizzez created by the user from the backend and will display 
  each created quiz in a separate "QuizCard" component.
->Each card of the quizzes will contain information related to the quiz, along with that 2 buttons to join the quiz and edit the quiz.
->When the user clicks on the join quiz button then "Quiz Display" component will get display.
->When the user clicks on the edit quiz button then "Questions" component will get display where user can add the questions again and can edit the quiz title and time.

Checking Quizzez Played-----
->When a user clicks on the joined Quizzez or joined button then "JoinedQuizzez" component(in Card folder) will get display. It will fetch the data of the quizzes played by the user from the backend and will 
  display each played quiz in a separate "QuizCard" component.
->Each card of the quizzez played will contain information related to the quiz along with that 2 buttons to join quiz and view results.
->When the user clicks on the join quiz button then "Quiz Display" component will get display.
->When the user clicks on the view results button then "JoinedQuizResult" component will get display.It will fetch the data of all the quizzes played by the user from the backend and will display it.
