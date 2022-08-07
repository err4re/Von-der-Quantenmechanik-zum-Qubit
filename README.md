# Von-der-Quantenmechanik-zum-Qubit


# 1. Installation

Für die Installation habt ihr zwei Optionen, entweder ihr installiert Anaconda (Python) und Jupyter Lab (Editor) lokal auf eurem Betriebsystem, oder ihr entscheidet euch dafür unsere Virtual Machine zu verwenden. Dieses von uns vorbereitete Betriebssystem läuft virtuell auf eurem PC und funktioniert garantiert, allerdings eben nur in VirtualBox (Virtualisierungssoftware). VirtualBox müsst ihr dann trotzdem installieren.

Das heißt also:

1. Option: lokale Installation von Anaconda, Jupyter Lab *(empfohlen)*
2. Option: VirtualBox installieren *(empfohlen wenn 1. fehlschlägt)*

## 1. Option: lokale Installation

### Python

Wir werden Python verwenden, weil dies in der Physik die mit Abstand am stärksten verbreitete Programmiersprache ist und weil IBM sie für ihre Quantencomputing Plattform verwendet. Außerdem ist sie einfach schön :star_struck:
Um Python zu installieren nutzen wir Anaconda, entweder mit GUI (graphic user interface) [hier](https://docs.anaconda.com/anaconda/install/) oder ohne ganz minimalistisch [hier](https://docs.conda.io/en/latest/miniconda.html), die Wahl überlassen wir euch. Auch in der Version mit GUI könnte ihr das Terminal nutzen und habt also keinen Nachteil in dieser Hinsicht :innocent: allein die Installation ist etwas größer.

### Environment

Nachdem ihr Anaconda und damit :snake: installiert habt, ist es Zeit ein environment (virtuelle Umgebung) für unseren Kurs zu erstellen. Das könnt ihr in der GUI erledigen oder bequem im Terminal *(empfohlen)*, fragt uns gerne nach Hilfe.

Los geht's, öffnet das (miniconda oder Anaconda) Terminal und verwendet die folgenden Befehle. Ihr könnt das Terminal einfach in der Suchleiste suchen. Und dann:

`conda create -n akademie2022 python=3`

Hier erstellen wir eine Umgebung mit dem Namen `akademie2022` und verwenden in dieser Umgebung Python 3 (niemand will mehr Python 2 und so sind wir uns sicher, dass es nicht peinlich wird). Ihr könnte gerne auch einen anderen Namen als `akademie2022` verwenden, das liegt bei euch. Aber jetzt ist es wahrscheinlich zu spät :joy:

Kurzes Update:

`conda update conda`

Als nächstes aktivieren wir die neue Umgebung, das heißt wir wechseln in diese Umgebung:

`conda activate akademie2022`

Ihr solltet jetzt neben eurem Cursor so etwas wie `(akademie2022)` sehen. Dann kann es jetzt mit den interessanten packages (Erweiterung für Anaconda und/oder Python) los gehen.

Wir beginnen mit [Jupyter Lab](https://jupyter.org), einem Editor für :snake: (und viele andere Programmiersprachen), den ihr heute Vormittag schon gesehen habt. 

Jetzt Jupyter Lab installieren:

`conda install jupyterlab`

Stimmt jetzt bitte allen Abfragen zu zusätzlichen packages zu (und im weiteren Verlauf genauso :sweat_smile:). Ok das hat hoffentlich geklappt, ansonsten fragt bei uns nach.

Weiter geht es mit ein paar Python libraries (Bibliotheken mit nützlichen Funktionen, die wir nicht selber schreiben wollen und können :dizzy_face:). Für die Mathe:

`conda install numpy`

Für die Graphen (habt ihr heute schon in Aktion gesehen):

`conda install matplotlib`

Für die Quatencomputer :raised_hands: :

`pip install qiskit`

Quantencomputer können schöne Graphen vertragen:

`pip install qiskit[visualization]`

Uuuuuuuund das war's für erste an Installationen, Glückwunsch ihr habt es geschafft! :v:

## 2. Option: VirtualBox


Einfach [VirtualBox](https://www.virtualbox.org/wiki/Downloads) installieren und bei uns nach der Distribution fragen :wink:

# 2. Erste Notebooks

Dann starten wir zum ersten Mal unser frisches Jupyter Lab:

`jupyter lab`

Hier könnt ihr jetzt ein neues Notebook erstellen, zum Beispiel unter **File>New>Notebook**. Schaut euch als erstes die Bibliothek `matplotlib` an, genaueres dazu [hier](https://matplotlib.org/). Falls ihr euch ein Beispiel anschauen möchtet, findet ihr in diesem repository (Git-Verzeichnis) auch das Notebook zur [UV-Katastrophe](https://github.com/err4re/Von-der-Quantenmechanik-zum-Qubit/blob/main/UV_Katastrophe.ipynb).

Hier eine kleine Aufgabenlist:

1. definiere eine lineare Funktion
2. plotte den Graphen dieser Funktion
3. gib dem Plot eine Überschrift
4. definiere ein Potenzgesetz und erstelle einen analogen Plot
5. erstelle außerdem einen doppelt-logarithmischen Plot
6. erstelle einen interaktiven Plot für eine Potenzgesetz mit variablem Koeffizienten, das heißt der Koeffizient kann interaktiv verändert werden

Zusätzliche Informationen zu `matplotlib` findet ihr [hier](https://matplotlib.org/stable/tutorials/index.html).

Ansonsten gerne noch `qiskit` testen, im notebook:

```
import qiskit
qiskit.__version__
```