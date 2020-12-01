# Multi-Instance-Prozess

Dieser Prozess zeigt, wie Sie eine Mehrfachausführung einer Benutzeraktivität verwenden können.

Beim Prozessstart muss die Variable `performers` übergeben werden.
Diese Variable enthält ein Array von Identitäten.
Die entsprechenden Anwender bekommen im Verlauf des Prozesses eine Aufgabe zugewiesen.
Sobald alle Anwender ihre Aufgabe abgeschlossen haben, ist der Prozess beendet.
