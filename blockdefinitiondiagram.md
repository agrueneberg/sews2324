# BDD autonomes Fahrzeug

![blockdefinitiondiagram-01.drawio.png](blockdefinitiondiagram-01.drawio.png)

Im Zentrum des Systems steht das **Fahrzeug** als Komponente.\
Das Ziel, wohin das **Fahrzeug** fahren soll, erhält es über das **Zielbestimmungsinterface**.\
Die **Planung** bestimmt, anhand der **Sensorik**, wie die **Aktorik** angesteuert werden muss, um zum Ziel zu gelangen.\
Die **Sensorik** besteht zum einen aus Sensoren um Informationen über das Fahrzeug selbst zu messen (**Selbstwahrnehmung**), wie die aktuelle Position, und Sensoren um das Umfeld wahrzunehmen (**Umfeldwahrnehmung**), um zum Beispiel Hindernisse zu erkennen.\
Es gibt verschiedene Instanzen von der Selbstwahrnehmung und der Umfeldwahrnehmung, z.B. ist der Ultraschallsensor eine Instanz der Umfeldwahrnehmung. Die Sensorik ist daher eine Sammlung von Sensoren und fusioniert die Sensordaten.\
Die Aktorik besteht aus einem **Motor**, **Bremsen** und einer **Lenkung**.
