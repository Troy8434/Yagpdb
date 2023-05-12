<h1>Useful</h1>
<h2>Image only</h2>
Der Image only Code funktioniert am besten mit einem Regex Tigger, welcher in diesem Beispiel <b>.*</b> ist. 
Der Custom Command mit dem Image only Code löscht alle Nachrichten, die keine Bilder / Videos beinhalten. Daher sollte er nur auf wenige Channel begrenzt werden, falls ihr nicht den ganzen Server lahmlegen möchtet. Dies eignet sich z.B. für Meme Channels in denen keine Kommentare erwünscht sind. Zur Bewertung der Memes können auch Reaktionen hinzugefügt werden.

<h2>Tickt Reaction</h2>
Hier ist eine einfache Möglichkeit ein Ticket per Reaktion zu öffnen. 
Der Code funktioniert mit einem <b>Reactions: add only</b> Trigger und öffnet ein neues Ticket, wenn ein User mit 📩 auf eine im Code festgelegte Nachricht reagiert.
Die Nachricht wird durch eine ID (hier 763004687532163082) und einen Titel (hier **How to Partner**) spezifiziert. Außerdem muss es sich bei der Nachricht um ein Embed handeln, damit dieser Code funktioniert. 

Tipp:
Ihr könnt <b>{{addMessageReactions nil 763004687532163082 "📩"}}</b> nutzen um den Bot eine Reaktion hinzufügen zu lassen, sodass User diese nur noch antippen müssen.
Dazu muss der oben gezeigte Code in einem Custom Command in dem Channel ausgelöst werden, in dem sich die Nachricht befindet. Die ID der Nachricht muss auch hier wieder ausgetauscht werden. Optional könnt ihr auch nil durch die ChannelID des Channels welcher die Nachricht beinhaltet austauschen, was es euch ermöglicht den Code auch von anderen Channels aus zu triggern. Dieser Code muss nur einmal getriggert werden.