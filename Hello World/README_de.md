# Hello-World-Prozess

Dieser Prozess zeigt, wie Benutzeraufgaben als "User Task"-Elemente in einem Prozess modelliert werden können.

Wenn ein Prozess ein "User Task"-Element erreicht, wird eine Aufgabe in d.ecs task erstellt.
Der Wert des Attributs `name` im "User Task"-Element wird zum Betreff der Aufgabe.
Wem die Aufgabe zugewiesen wird, entscheidet sich anhand der verwendeten Benutzerzuordnung in der Benutzeraufgabe. Aufgaben werden entweder einem einzelnen Benutzer zugeordnet (camunda:assignee) oder mehreren Empfängern zugewiesen (camunda:candidateUsers).

Der vorliegende Prozess besteht aus einer einzigen Benutzeraufgabe.
Wenn der Prozess gestartet wird, wird eine Aufgabe mit dem Betreff "Hello World" in d.ecs task erstellt.
Diese Aufgabe wird dem Prozessstarter zugewiesen, da er über die Prozessvariable `dv_initiator` als "camunda:assignee" in der Benutzeraufgabe modelliert ist.
Wenn der Prozessstarter die Aufgabe abschließt, ist der Prozess beendet.
