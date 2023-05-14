<h1>Stundenplan</h1>
Der Stundenplan ist in 3 Teile aufgeteilt. Diese sind: Ein Tageszähler, ein Embed mit Informationen & den Reaktionen und die Abfrage der Fächer. Die Abfrage der Fächer musste aufgrund von einer zu langen Länge auf 2 Commands aufgeteilt werden.
Der Stundenplan kann jedem Schüler einer Klasse einen anderen Stundenplan basierend auf ihren Rollen ausgeben. Außerdem ist er für ein 2 Wochensystem ausgelegt.

<h2>Tageszähler</h2>
Der Tageszähler ist ein kurzer Code, welcher in einem <b>times Command</b> eingefügt werden sollte, welcher sich alle 24 (und am besten um Mitternacht) erneut ausführt.
Der Code zählt die Tage bis 14 und fängt danach wieder von vorne an. So weiß der Bot immer, ob es eine gerade / ungerade Woche ist und welcher Wochentag heute ist.
Der Tageszähler sollte außerdem an einem Montag in einer ungeraden Woche starten, da dieser hier die Nummer 1 hat.

<h2>Embed</h2>
Das Embed kann in einen Channel als kurze Erklärung gepostet werden. Vor allem aber wird hier der Stundenplan anhand von Reaktionen abgefragt. 1️⃣ steht hierbei für den heutigen Stundenplan und 2️⃣ für den morgigen. Diese Reaktionen werden bei dem Embed automatisch vom Bot hinzugefügt, sodass User diese nur noch anklicken müssen. Dieses Embed muss nur einmal gesendet werden. Dies kann z.B. durch einen einfachen Command Trigger geschehen.

<h2>Stundenplan</h2>
Der Hauptpart des Stundenplans ist die Abfrage der Fächer eines Users. Zu diesem Zweck geben wir den Usern für jedes von ihnen Belegte Fach / Kurs eine Rolle. Die ID dieser Rolle weisen wir einer Variable zu, die wir später im Code abfragen. Für den Zeitpunkt an dem ein Kurs stattfindet wird abgefragt, ob der User die Rolle dieses Kurses hat. Hat er eine der Rollen, die einem z.B. im zweiten Block an ungeraden Dienstagen stattfindenen Kurs entsprechen, so wird dieser Kurs für dies Zeit in einem Embed eingetragen. Sobald alle Kurse für den entsprechenden Tag (heute oder morgen) abgefragt sind, sendet der Bot eine DM Nachricht mit dem fertigen Embed, in dem alle Stunden eingetragen sind.
Da die Stundenabfrage zu lang für einen Custom Command ist, wird ein zweiter benötigt. Diesen triggern wir durch <b>{{execCC 78 nil 1 $x}}</b> falls der gewünschte Tag nich in einer ungeraden Woche sein sollte. Die 78 muss hierbei durch die ID des zweiten Custom Commands ersetzt werden. Je nachdem, welchen ihr für den zweiten Teil des Codes wählt. Die Variablen für die Rollen müssen hier erneut zugewiesen werden. Der Trigger für den zweiten Teil der Stundenabfrage kann <b>None</b> sein, da wir ihn nur durch andere Custom Commands ausführen lassen wollen. Der Trigger für den ersten Teil der Stundenabfrage sollte ein Reaction Trigger sein. Genauer gesagt: <b>Reaction: Add only</b>