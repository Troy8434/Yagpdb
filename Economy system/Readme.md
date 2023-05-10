<h1>Economy System</h1>
Das hier aufgeführte System besteht lediglich aus 3-4 funktionierenden Commands. Diese sind <b>-bal</b>, <b>-work</b>, <b>-dep</b> und die Lotterie.
Da ein Economy System nicht nur aus diesen 3-4 Commands bestehen kann, sind weitere nötige Command-Ideen weiter unten aufgelistet. Leider wurde das Projekt abgebrochen, bevor diese umgesetzt werden konnten.
Der optimale Trigger für diese Codes ist ein Command.

<h2>Bal</h2>
Der -bal Command gibt die Menge an Coins an, die der User, der den Command genutzt hat auf der Bank, im Portmonee und insgesamt hat.
Da das Projekt recht früh abgebrochen wurde, ist es nicht möglich den Bal Command für andere Nutzer zu benutzen (-bal @user). Dies kann aber recht leicht nachgerüstet werden.

<h2>Work</h2>
Der -work Command erlaubt es Usern Coins zu verdienen. Die Menge der Coins beträgt einen zufälligen Betrag zwischen 100 und 500. Dieser Betrag wird dem Portmonee des Users zugeschrieben von wo aus sie mit dem -dep Command zur Bank gebracht werden können.
Der Work Command ist außerdem mit einem Cooldown von 2 Stunden ausgestattet, welcher sicherstellt, dass User nicht zu schnell an neue Coins kommen.

<h2>Dep</h2>
Der -dep Command ist dafür zuständig die Portmonee Coins eines Users auf die Bank zu bringen.
Er kann mit verschiedenen Argumenten verwendet werden, wie z.B. <b>-dep 1003</b> oder <b>-dep all</b>.
So kann ein User entweder einen bestimmten Betrag, oder alles was er im Portmonee hat zur Bank bringen.

<h2>Lotterie</h2>
Die Lotterie besteht aus 2 Teilen. Der erste Part (Lotterie Lose) kann als Command z.B. <b>-buy Lotterielos</b> benutzt werden. Dieser fügt den User zu der Lotterie hinzu.
Bei diesem Command fehlt allerdings noch der Teil, der dem User die Coins abzieht, die er für das Los bezahlt hat. Dieser kann auch mit ein wenig inspiration vom Dep Command nachgerüstet werden.
Der zweite Part der Lotterie (Lotterie Gewinner) kann entweder als ein timed Command existieren, welcher z.B. jede Woche ausgelöst wird, oder als ein Command, dessen Nutzung allerdings nur den Admins / Serverteam vorbehalten sein sollte (Was bei Custom Commands unten rechts eingestellt werden kann). Dieser Command zieht einen zufälligen User, der sich ein Lotterielos gekauft hat. Der Teil, der dem User die Coins überweist, muss auch hier wieder nachgerüstet werden.
Kauft ein User mehrere Lose, so erhöhen sich auch seine Gewinnchancen.