Ultraschallbad Einweisung
=========================

Einweisung des [FAU FabLab](https://fablab.fau.de) in das [Ultraschallbad](https://fablab.fau.de/tool/ultraschallbad/) Emag Emmi-30HC.

Inhalt
------

- Allgemeine Sicherheitshinweise mit Sicherheitszeichen (ISO 7010) und GHS-Piktogramm auf der ersten Seite
- Inhaltsverzeichnis und Arbeitsablauf als Grafik
- Das Gerät: technische Daten, Funktionsweise, was hinein darf, Bedienpanel, Zeitschalter
- Vorbereitung, Reinigen, Nach der Reinigung (Befüllen, Reiniger, Entgasen, Einlegen, Entleeren)
- Tipps, Störungen und Erste Hilfe, Infos für Betreuer
- Betriebsanweisung Gefahrstoff für den Ultraschallreiniger EMAG EM-080 (BA-GS-02) auf der letzten Seite,
  zusätzlich als eigenes PDF zum Aushang

Die Hinweise aus der Bedienungsanleitung von EMAG sind in eigenen Worten wiedergegeben, die Grafiken
(`zeichnungen/`) sind eigene TikZ-Zeichnungen.

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/ultraschallbad-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/ultraschallbad-einweisung/Einweisung_Ultraschallbad.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/ultraschallbad-einweisung/Einweisungsliste_Ultraschallbad.pdf)
- [Betriebsanweisung Ultraschallreiniger](https://brain.fablab.fau.de/build/ultraschallbad-einweisung/Betriebsanweisung_Ultraschallreiniger.pdf)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/ultraschallbad-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/ultraschallbad-einweisung.git
cd ultraschallbad-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/ultraschallbad-einweisung/status.svg)](https://brain.fablab.fau.de/build/ultraschallbad-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/ultraschallbad-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/ultraschallbad-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/ultraschallbad-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/ultraschallbad-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
