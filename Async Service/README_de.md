# Async-Service-Prozess

Dieser Prozess zeigt, wie ein asynchroner externer Service aufgerufen wird.

Als Beispiel dient der in d.velop process enthaltene asynchrone "Hello World"-Service.
Der Service kann über die URI `/process/services/helloworld/async` aufgerufen werden.
Er erwartet eine Input-Variable namens `yourName` und gibt eine Output-Variable namens `greeting` mit dem Wert "Hello <yourName>" zurück.

In diesem Beispielprozess wird zunächst der "Hello World"-Service aufgerufen.
Als Input-Variable `yourName` wird der Name des Prozessstarters übergeben.
Danach bleibt der Prozess stehen, bis die Antwort des Services eintrifft.
Die vom Service erhaltene Output-Variable `greeting` wird der gleichnamigen Prozessvariable `greeting` zugeordnet.
Der Prozess enthält nach Aufruf des Services eine Prozessvariable namens `greeting` mit dem Wert "Hello <Name des Prozessstarters>".
Diese Prozessvariable wird als Name für die folgende Benutzeraufgabe (User Task) verwendet, sodass der Prozessstarter eine Aufgabe mit dem Betreff "Hello <Name des Prozessstarters>" erhält.
Nach Abschluss der Aufgabe ist der Prozess beendet.
