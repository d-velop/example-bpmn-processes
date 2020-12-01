# Sync-Service-Prozess

Dieser Prozess zeigt, wie ein synchroner externer Service aufgerufen wird.

Als Beispiel dient der in d.velop process enthaltene synchrone "Hello World"-Service.
Sie können den Service über die URI `/process/services/helloworld/sync` aufrufen.
Er erwartet eine Input-Variable namens `yourName` und gibt eine Output-Variable namens `greeting` mit dem Wert "Hello <yourName>" zurück.

In diesem Beispielprozess wird zunächst der "Hello World"-Service aufgerufen.
Dabei wird als Input-Variable `yourName` der Name des Prozessstarters übergeben.
Die vom Service erhaltene Output-Variable `greeting` wird zur gleichnamigen Prozessvariable `greeting` zugeordnet.
Der Prozess erhält dadurch nach Aufruf des Services eine Prozessvariable namens `greeting` mit dem Wert "Hello <Name des Prozessstarters>".
Diese Prozessvariable wird in der folgenden Benutzeraufgabe ("User Task") als Name verwendet, sodass der Prozessstarter eine Aufgabe mit dem Betreff "Hello <Name des Prozessstarters>" erhält.
Nach Abschluss der Aufgabe ist der Prozess beendet.
