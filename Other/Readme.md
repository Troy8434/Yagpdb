<h1>Other</h1>
Dieser Unterordner ist eine Sammlung verschiedener Nebenprojekte, welche zumeist nur kurze Verwendung fanden. 
Diese sind: Ein digitaler Adventskalender, ein mathematisches Experiment und ein Valentinstagsbrief. 

<h2>Adventskalender</h2>
Der Adventskalender besteht aus zwei Commands. Der Counter muss, so wie bei dem Stundenplan, auch in einen 24 Stunden timed Command um ordentlich zu funktionieren. Vorzugsweise wird dieser auch um Mitternacht gestartet. 
Der Hauptteil des Adventskalenders kann in einem einfachen Command wie z.B. <b>-open</b> ausgeführt werden. Dieser sendet, sobald das Türchen geöffnet wird ein im Code für diesen Tag definiertes Bild in einem netten Embed. Es kann nur das Türchen für den heutigen Tag geöffnet werden und dies kann auch nur einmal pro Tag geschehen.

<h2>Zufallsziehung</h2>
Die Zufallsziehung ist ein Command, welcher z.B. alle paar Minuten mit einem timed Command ausgeführt werden kann. Er gibt eine Nachricht aus, sofern die Zufallsziehung eine Kombination wie ROT, TOR oder TRO bietet. Dieser Code basiert auf einer Zufallsziehung mit zurücklegen, für die drei Kugeln T, O, und R. 

<h2>Send a letter</h2>
Unter diesem Namen sammeln sich mehrere einzelne Commands, welche in einem Valentinstagsevent dazu benutzt wurden einen Brief an einen anderen User zu designen. 
So startet ein User, der einen Brief schreiben möchte damit einen neuen Channel zu eröffnen. 
In diesem Channel kann der User die Art, das Papier, die Schrift, eventuelle Sticker, einen Empfänger, einen Sender und natürlich den Text auswählen.
Dies geschieht mit je einem Command für die einzelnen Sachen. Angafangen wird mit der Art des Briefes (Freundschaftsbrief oder Liebesbrief). Der vorgesehende Command hierfür würde z.B.<b>-art Freundesbrief</b> lauten. Da "Freundesbrief" ein Argument ist, muss der Command in den Einstellungen nur <b>-art</b> lauten. Wichtig ist hier, dass der Command <b>-art</b> den nächsten Schritt triggern soll. Also muss dieser Command den Code von der Briefart beherbergen. Dieser speichert die ausgewählten Werte und gibt Anweisungen, wie der User weiter fortfahren kann. In diesem Fall mit der Papierart.
So geht es weiter, bis alle Punkte abgearbeitet sind. Nachdem der User fertig ist, kann er die gesammelten Werte mit dem Submit und Delete Entries Code an das Serverteam weitergeben. Dies kann z.B. über einen einfachen Command wie <b>-submit</b> geschehen. Das Serverteam kann dann basierend auf den ausgewählten Werten des Users einen Brief herstellen und diesen am Valentinstag veröffentlichen. 
