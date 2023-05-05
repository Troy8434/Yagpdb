<section>
    <h1>Bot Interaktionen</h1>
    <details>
        <summary>
            <h2>Feed</h2>
        </summary>
        Feed wird als Command Trigger empfohlen. Der Command kann mit, aber auch ohne folgende Argumente verwendet werden. Sollten keine Argumente kommen (z.B. <b>-feed </b>), so wird eine zufällige Nachricht Nachricht aus dem Code ausgewählt. Sollte ein Argument vorhanden sein (z.B. <b>-feed Kekse</b>) wird dieses Argument in die Antwort mit eingebunden.
    </details>
    <details>
        <summary>
            <h2>Say</h2>
        </summary>
        Say funktioniert ähnlich wie der Feed Command. Hier ist ein Argument aber Pflicht. Das heißt, dass der Bot bei dem Command <b>-say gib mir mal die Kekse</b> einfach das Argument (gib mir mal die Kekse) wiedergibt und den Trigger löscht. Dies kann zu lustigen Konversationen beitragen, aber auch missbraucht werden um Moderationsfilter zu umgehen. Also Vorsicht. 
        Der Command hat außerdem einen Cooldown eingebaut, der das Spammen verhindert. Dieser kann bei Bedarf verändert werden. (z.B. $lengthSec = 1)
    </details>
    <details>
        <summary>
            <h2>Speisekarte</h2>
        </summary>
        Als Trigger für die Speisekarte ist ein "Starts with" Trigger empfohlen. Dieser kann, um mit der Speisekarte sinnvoll verwendet werden zu können, z.B. "Bring mir" sein.
        Beispiel: <b>Bring mir Popcorn</b>. Ist das Argument im Command definiert, so gibt der Bot eine vorgefertigte Antwort aus. Sollte das Argument nicht im Code auftauchen, wird es ähnlich wie beim Feed in eine Nachricht eingefügt.
    </details>