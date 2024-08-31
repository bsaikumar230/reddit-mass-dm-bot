# In action!
![In action!](https://github.com/bsaikumar230/reddit-mass-dm-bot/blob/main/media/InAction!.png)

# In progress
Add a UI(User Interface). I haven't started working on this, I think the bot will remain a CLI-only tool for now.

# Prerequisites
0 - Have ```Python``` and ```Pip``` installed. This project was developed with Python 3.11.8<br>
1 - Clone this repository.<br>
2 - Install ```Pipenv``` using the command ```pip install pipenv```.<br>
3 - Run ```pipenv install``` inside the project to install its dependencies.<br>
4 - Run ```playwright install Chromium``` or ```python -m playwright install Chromium``` to install Playwright dependencies(browser).<br>

# How to use
1 - Add accounts to ```rdt/account.json```.<br>
2 - Change what needs to be changed in ```rsrc/config.json```.<br>
3 - Fill ```db/usernames.csv``` with all the usernames you want to DM.<br>
4 - Run ```RedditDMBot.py```.<br>

# How does it work?
RedditDMBot is a bot made for the purpouse of automating the process of sending messages to Reddit users<br>
What the bot does:<br>
0 - The bot checks whether you have a proxy in ```rsrc/config.json```, all actions will be made through the proxy if found.<br>
1 - Logs into one of the Reddit account in ```accounts.json```.<br>
2 - Navigates to chat page.<br>
3 - Checks if the user already received a message.<br>
4 - Sends a message to the user.<br>
5 - Deletes the user from the list of users to DM and adds it to ```db/usernames_sent.csv```.<br>
6 - Logs out of the account used to DM the user.<br>
7 - Remove it from the list of available accounts and add it to a list of used accounts.<br>
8 - Logs into another Reddit account that wasn't used.<br>
9 - If there are no many available accounts, the bot reuses the used accounts until all users on your ```db/usernames.csv``` received DMs.

<br><br>
Enjoy!
