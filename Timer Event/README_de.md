# Timer-Event-Prozess

Dieser Prozess zeigt, wie ein Timer-Ereignis verwendet werden kann.

Beim Start des Prozesses wird dem Prozessstarter eine Aufgabe mit dem Betreff "Hello World" zugestellt.
Schließt der Prozessstarter die Aufgabe nicht innerhalb von einer Minute ab, wird das Timer-Ereignis ausgelöst.
Daraufhin wird die Aufgabe gelöscht und der Prozess läuft durch den Sequenzfluss `s3` zum Endereignis.
