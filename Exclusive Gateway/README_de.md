# Exclusive-Gateway-Prozess

Dieser Prozess zeigt, wie ein exklusives Gateway verwendet werden kann.

Beim Start des Prozesses muss die Variable `amount` mitgegeben werden.
Je nach Wert der Variablen entscheidet sich am ersten Gateway, welchen Pfad der Prozess durchläuft.
Ist der Wert der Variablen größer als 1000, durchläuft der Prozess den Sequenzfluss `gateway-option-a` und dem Prozessstarter wird eine Aufgabe mit dem Betreff "Hello World" zugewiesen.
Im anderen Fall durchläuft der Prozess den Sequenzfluss `gateway-option-b`, der keine Bedingung hat, sondern als Default markiert ist, und der Prozess wird direkt beendet.
