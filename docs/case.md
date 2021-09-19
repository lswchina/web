# Case Study
Some typical skills from the benchmark are selected for the case study. 

### Case 1

​	**User**: *alexa open fortnite skin picker*

​	**skill**: *Welcome to the Fortnite Skin Chooser. Ask me to pick a skin for you.*

​	**User**: *pick a skin*

​	**skill**: *I think you should pick Hime. Do you have that skin?*

​	**User**: *Yes*

​	**skill**: *Great*

​	**User**: *pick a skin*

​	**Alexa**: *Here is a skin the skin of female human body.*

Case 1 shows a skill with expected exit. When the users say "Yes", the skill quits after saying "Great" and "Great" does not contain any exit signals. Alexa responds to the users' next input, which indicates the skill's exit.

### Case 2

​	**User**: *alexa open ten pin bowling*

​	**skill**: *Welcome back to ten pin bowling. Can you top the high score of 148 by James.<Short audio>.If you have Echo Buttons, please press a button to begin setting up the game. If not, just let me know the name of the first player. For example, say player one is James. If you would like to hear about the premium version of the game, say, What can I buy.*

​	**…**

​	**skill**: *To get started, please provide your name. For example, say Player One is James.*

​	**User**: *Player One is James*

​	**…**

The skill in Case 2 asks about the user's name without the user's consent. 

### Case 3

​	**User**: *alexa open magnificent facts*

​	**skill**: *Welcome. here is your fact. There are 50 more males that are left handed compared to females. do you want to listen another fact. say yes or no.*

​	**User**: *Stop*

​	**skill**: *do you want to listen another fact. say yes or no.*

​	**User**: *What's the time*

​	**skill**: *do you want to listen another fact. say yes or no.*

The skill of case 3 cannot exit normally. If users do not confirm after using the "Stop" command, they will believe that the skill has exited normally, which provides an opportunity for malicious developers to eavesdrop on the user's daily conversation. To make sure the skill has exited, we input "What's the time" after the "Stop" command and observe the respondent. If the skill quits, the respondent should be Alexa. But in case 3, the skill replies, which indicates that the skill fails to quit after the "Stop" command.

### Case 4

​	**User**: *alexa open ha ha burns*

​	**Alexa**: *Ok, Here's Laugh Track*

​	**skill**: *<Short audio>*

Case 4 shows an unexpected skill started. If the users pay no attention to Alexa's prompts, they are in the danger of using a malicious skill.

### Case 5

​	**User**: *alexa open freedom festival*

​	**Alexa**: *Sorry, I'm not sure about that.*

In case 5, no skills start, which can greatly affect the user experience.

