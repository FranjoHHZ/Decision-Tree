# Decision-Tree

In diesem Notebook wird eine Entscheidungsbaum- und Random Forest-Klassifikation verwendet, um vorherzusagen, ob ein Kreditnehmer bei LendingClub.com einen Kredit zurückzahlen wird oder nicht. Die Daten umfassen verschiedene Merkmale der Kreditnehmer, die zur Vorhersage verwendet werden können. Das Ziel besteht darin, ein Modell zu erstellen, das anhand dieser Merkmale die Rückzahlung des Kredits vorhersagt. Wir werden Daten von 2007 bis 2010 verwenden, bevor das Unternehmen an die Börse ging. Anhand der Daten werden wir versuchen vorherzusagen, ob ein Leihender das Geld zurückgezahlt hat oder nicht.  

# Ausführung
Um dieses Jupyter Notebook auszuführen, müssen Sie dem Link des oben genannten Binder-Badges folgen. Öffnen Sie das Notebook „3-Logistische_Regression_Projekt-Loesung.ipynb“. Sobald das Notbook geöffnet wurden, gehen Sie bitte auf den Reiter "Edit" und drücken Sie "Clear Outputs of all Cells". Nachdem Sie das gemacht haben, können Sie auf "Run all Cells" klicken um den Code auszuführen.

Schritte im jupyter Notebooks
Daten laden und erkunden: Die Daten werden aus einer CSV-Datei in einen Pandas DataFrame geladen. Dann werden grundlegende Informationen über die Daten angezeigt, wie z. B. die Anzahl der Beobachtungen und die Datentypen der Spalten. Die info() und describe() Methoden helfen dabei, einen ersten Überblick über die Daten zu gewinnen.

Datenaufbereitung und -bereinigung:

Die Daten werden auf fehlende Werte überprüft und notwendige Bereinigungen durchgeführt. Dies könnte das Entfernen oder Ersetzen von fehlenden Werten umfassen.
Kategorische Variablen wie die Spalte purpose werden in numerische Dummy-Variablen umgewandelt, da maschinelle Lernmodelle nur numerische Daten akzeptieren.
Trainings- und Testdaten aufteilen:

Die Daten werden in Trainings- und Testsets aufgeteilt, um das Modell zu trainieren und später zu evaluieren.
Die unabhängigen Variablen (Features) umfassen alle numerischen Spalten (einschließlich der Dummy-Variablen für purpose), während die abhängige Variable die Spalte credit.policy ist, die angibt, ob ein Kreditnehmer die Risikobewertung bestanden hat.
Modelltraining:

Entscheidungsbaum-Modell: Ein Entscheidungsbaum wird auf dem Trainingsset trainiert, um die Beziehung zwischen den Merkmalen und der Rückzahlungswahrscheinlichkeit zu lernen.
Random Forest-Modell: Ein Random Forest-Modell, das aus mehreren Entscheidungsbäumen besteht, wird ebenfalls auf den Trainingsdaten trainiert. Random Forests sind in der Regel robuster und genauer als einzelne Entscheidungsbäume, da sie mehrere Bäume kombinieren und die Ergebnisse aggregieren.
Vorhersagen und Evaluierung:

Die Modelle werden verwendet, um Vorhersagen auf dem Testset zu machen.
Die Vorhersagen werden mit der tatsächlichen Rückzahlung verglichen, um die Modellleistung zu bewerten. Dies geschieht durch Berechnung der Precision, Recall, F1-Score, und der Accuracy.
Ergebnisse anzeigen:

Die Confusion Matrix zeigt, wie viele positive und negative Fälle korrekt und inkorrekt vom Modell vorhergesagt wurden.
Ein Classification Report liefert eine detaillierte Bewertung der Modellleistung.

# Ergebnisse

In diesem Projekt wird die explorative Datenanalyse (EDA) eingesetzt, um ein umfassendes Verständnis der Datenstrukturen zu erlangen. Dazu gehören auch visuelle Darstellungen wie Histogramme, die die Verteilung bestimmter Merkmale aufzeigen. Diese Visualisierungen sind wichtig, um Muster und Zusammenhänge in den Daten zu entdecken, die die Vorhersagegenauigkeit der Modelle beeinflussen können.

Das Hauptziel des Projekts besteht darin, mithilfe von Decision Trees und Random Forests ein Modell zu erstellen, das eine hohe Genauigkeit bei der Klassifizierung erreicht. Die Leistungsfähigkeit der Modelle wird durch Metriken wie Genauigkeit, Präzision, Rückruf und F1-Score bewertet.


# Binder Badge
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FranjoHHZ/Decision-Tree/master?labpath=3-Decision_Trees_und_Random_Forests_Projekt-Loesung.ipynb)
