# Von-der-Quantenmechanik-zum-Qubit


# 1. Installation

Für die Installation habt ihr zwei Optionen, entweder ihr installiert Anaconda (Python) und Jupyter Lab (Editor) lokal auf eurem Betriebsystem, oder ihr entscheidet euch dafür unsere Virtual Machine zu verwenden. Dieses von uns vorbereitete Betriebssystem läuft virtuell auf eurem PC und funktioniert garantiert, allerdings eben nur in VirtualBox (Virtualisierungssoftware). VirtualBox müsst ihr dann trotzdem installieren.

Das heißt also:

1. Option: lokale Installation von Anaconda, Jupyter Lab *(empfohlen)*
2. Option: VirtualBox installieren *(empfohlen wenn 1. fehlschlägt)*

## 1. Option: lokale Installation
------

### Python

Wir werden Python verwenden, weil dies in der Physik die mit Abstand am stärksten verbreitete Programmiersprache ist und weil IBM sie für ihre Quantencomputing Plattform verwendet. Außerdem ist sie einfach schön :star_struck:
Um Python zu installieren nutzen wir Anaconda, entweder mit GUI (graphic user interface) [hier](https://docs.anaconda.com/anaconda/install/) oder ohne ganz minimalistisch [hier](https://docs.conda.io/en/latest/miniconda.html), die Wahl überlassen wir euch. Auch in der Version mit GUI könnte ihr das Terminal nutzen und habt also keinen Nachteil in dieser Hinsicht :innocent: allein die Installation ist etwas größer.

### Environment

Nachdem ihr Anaconda und damit :snake: installiert habt, ist es Zeit ein environment (virtuelle Umgebung) für unseren Kurs zu erstellen. Das könnt ihr in der GUI erledigen oder bequem im Terminal, fragt uns gerne nach Hilfe.

Los geht's, öffnet das Terminal und verwendet die folgenden Befehle:

`conda create -n akademie2022 python=3`

Hier erstellen wir eine Umgebung mit dem Namen `akademie2022`

