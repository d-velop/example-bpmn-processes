# Escalation-Prozess

Dieser Prozess zeigt, wie eine Eskalation modelliert werden kann.

Wenn der Prozessstarter die Aufgabe "Hello World" nicht innerhalb von einer Minute abschließt, wird das angeheftete Timer-Ereignis ausgelöst und die Aufgabe abgebrochen (siehe Beispielprozess "Timer Event").
Nun löst der Prozess das Eskalationsereignis `throw_time_escalation` aus.
Dieses Ereignis ist über die Eskalationsdefinition `time_escalation` mit dem Startereignis `sub_start` des Subprozesses verknüpft, sodass der Subprozess gestartet wird.
Innerhalb des Subprozesses wird dem Prozessstarter eine Aufgabe mit dem Betreff "Escalation occurred" zugewiesen.
