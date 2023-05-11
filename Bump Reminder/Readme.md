<h1>Bump Reminder</h1>
The Bump reminder is one of the more prised creations and since you won't receive much help with bump reminders from the community, it's also quite rare. 
This one is based on reactions. Since YAGPDB can't react to messages of other bots, we use reactions as a trigger. Add Reactions only to be exact. 
This reaction trigger will execute the first part of the code. If a :bell: Emoji is added as a reaction to a successful bump message from Disboard the reminder will be activated.
The Code will detect when the successful Bump message was send and calculate when the next bump can be done. 
It will then execute another custom command. (In this example it's custom command number 16.) <b>You'll have to change this number to the custom command you'll use for the second part of the code</b>.
The second part of the code, as mentioned, get's it's own custom command (in this case with the number 16). Since the code is executed through another command, it is advised not to set any triggers.
There are also two risks about this code design:
1) When adding the :bell: to a bump done message which is older than 2 hours, the reminder will send a message instantly. This can be quite confusing when someone adds the reaction to the wrong message or it could even lead to spam.
2) Sometimes when YAGPDB is offline during an active reminder, you'll need to reset the remind by hand. 
This can be achieved easily by creating a new custom command with the code <b>{{dbDel (toInt64 0) "Bumps"}}</b>. This resets the reminder and you'll be able to restart it by adding the :bell: again. This line of code should only be executable by admins.