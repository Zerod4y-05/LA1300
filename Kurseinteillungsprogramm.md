# Kurseinteilungsprogramm

## Aufgabenstellung und Ziele

Das Programm soll Personen auf Kurse einteillen, und die 1., 2. und 3. wahl beachten. Das Progtamm gitb dann eine Liste aus, wer welchen Kurs besucht.

1. Der Leser soll nach dem Eintrag verstehen wie While-schleifen ohne einen Bool beendet werden kann.

## Text + Code Zeile
While-schleifen haben ein relativ einfaches Prinzip, doch auch mit den einfachsten Mitteln hat man viele verschiedene anwendungsmöglichkeiten.
```csharp
while (true)
            {
                try
                {
                    counter = 0;
                    Console.Write(question);
                    cours = Console.ReadLine();

                    for (int i = 0; i < allCourses.Length; i++)
                    {
                        if (cours != allCourses[i])
                        {
                            counter++;
                        }
                    }

                    if (counter == allCourses.Length)
                    {
                        throw new Exception();
                    }

                    break;
                }
                catch (Exception)
                {
                    Console.ForegroundColor = ConsoleColor.DarkRed;
                    Console.WriteLine("Dies ist kein Kurs.");
                    Console.ForegroundColor = ConsoleColor.White;
                }

            }
```
Hier sieht man eine While Schleife mit dem einfachsten Boolean "True", dies bedeutet, dass es immer wahr ist und diese Schleife sollte ununterbrochen weiterlaufen. Doch diese Schleife läuft nicht ununterbrochen weiter, wieso nicht? Die Antwort liegt bei dem Break. Das Break verursacht folgendes: Falls die Zeile mit dem Break erreicht und ausgeführt wird, wird die While-schleife beendet und der Code ausserhalb der While-Schleife wird ausgeführt. Diese Methode zu verwenden ist effektiv, falls man keinen Bool verwenden kann, um die While-schleife aufzulösen. Doch bevor das Break erreicht werden kann, muss es Hindernisse geben, welche zuerst erfüllt/nicht erfüllt werden müssen. In diesem Beispiel wäre das, das Try-catch, die For-schleife, und das If Statement. So kann alles gründlich ausgeführt werden ohne dass man die While-schleife vorzeitig beendet.

## Screenshot
![grafik](https://user-images.githubusercontent.com/89130485/142179644-1a0593ac-5f6d-4b20-9ed8-05366dca2577.png)

## Video
https://youtu.be/cLsgOMfSQTk

## Verifikation + Reflektion
Verifikation:
Ich habe diese Ziele Erreicht
Ziel 1: Wird mit dem Video, Screenshot und textlicher Beschreibung + Code Snippets erklärt.

Reflektion:
Bei diesem Projekt habe ich viel Zeit in die Projektdokumentation investiert, und konnte somit nicht so viel Programmieren wie meine Gruppenmitglieder, doch ich habe auch meinen Beitrag geleistet.
