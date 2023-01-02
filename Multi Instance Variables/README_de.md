# Multi-Instance-Prozess mit Variablen

Dieser Prozess zeigt, wie Sie in einer Mehrfachausführung eines Subprozesses Variablen im Prozess ändern können.

Beim Prozessstart muss die Variable `allAssignees` übergeben werden.
Diese Variable enthält ein Array von Identitäten.
Die entsprechenden Anwender bekommen im Verlauf des Prozesses eine Aufgabe zugewiesen.
Sobald ein Anwender seine Aufgabe beendet und die lokale Variable `decision` mit einem Wert belegt hat, wird dieser Wert in die globale Variable `allDecisions` geschrieben.
Sobald alle Anwender ihre Aufgabe abgeschlossen haben, ist der Prozess beendet.
