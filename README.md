Download Link: https://assignmentchef.com/product/solved-cpts479-assignment-12
<br>
For this homework you will create a version of the Quiz App that displays the questions in 3D as they move off into the distance like the introductory stories in the Star Wars films, all while playing the Star Wars theme music. A Next button will cycle through the questions. A video of the app in action is at <u>https://www.eecs.wsu.edu/~holder/courses/MAD/hw12/QuizAppHW12.mp4</u>. See screen shots below. Specifically,

<ol>

 <li>Create a new Single View project, embed the view in a Navigation Controller, and set the title and prompt in the navigation bar. Drag in a SceneKit View and set its auto layout constraints to the edge of the navigation bar at the top and the edge of the view at the bottom, left and right. Add an outlet to this SceneKit View to the ViewController.</li>

 <li>Add a SceneKit Scene File to the project and name is “QuizScene.scn”. In the scene editor add two 3D Text objects: one for the question and one for the Next button. You will need to modify the color, position and angle of these 3D Text objects either in the scene editor or programmatically.</li>

 <li>Similar to HW2, add a Question class to the project. In the ViewController, initialize a quiz array containing at least three questions. You may want to add some newlines ‘<strong>
</strong>’ in your question and answer strings if they are long, e.g., “The earth is which planet from the sun?.<strong>
</strong> This will be…”.</li>

 <li>Also similar to HW2, add a method for displaying a question with the question number, prompt, and all answers, each on a separate line. The question as a whole should be centered and start somewhere near the bottom of the screen. See the code snippet below for how I positioned the question once the whole thing is in the string quizString.</li>

</ol>




<ol start="5">

 <li>To the question text object add an infinitely-looping MoveBy action. You can tweak the dx/dy/dz and duration of the action to get the desired Star Wars effect.</li>

 <li>Create a Blink sequence action (fadeout, fadeIn) that is run on the Next text object whenever the user taps Next.</li>

 <li>Override the touchesEnded method to identify when the user taps the Next button. This should trigger the Blink action and advance to the next question, which should start at the bottom-center position again. Tapping Next on the last question should move to the first question in the quiz array.</li>

 <li>Finally, set up an AVAudioPlayer to continually loop through the Star Wars theme music. You can find an MP3 at <u>https://archive.org/details/StarWarsThemeSongByJohnWilliams</u> (see Download Options).</li>

 <li>We will test your app only in portrait mode on an iPhone 8 simulator, so the app does not have to adapt to different orientations or device sizes.</li>

 <li>And may the force be with you!</li>

</ol>







StoryBoard:







Scene Editor:




Simulator:


