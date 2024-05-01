---
layout: page
title: "Fragen die Fachleute"
class: home
mathjax: true
---

# Fragen die Fachleute

Dieses Modell verbindet zwei Ideen – lineare Regression und Domänenwissen.

## Domänenwissen

Domänenwissen ist Wissen, den Fachleute kennen.
Erfahrene Meinungen sind oft zutreffend, aber sie sind schwer in den Modellen zu verbinden, weil die Informationen nicht immer numerisch sind.
Kicker.de ist eine Quelle, die numerische erfahrene Informationen über die Note von Spieler und Teams verfügt.
Mit diesem Modell vergleichen wir die Notendifferenz von Kicker.de gegen die eigentliche Tordifferenz.
Wir berechnen diese Statistik so wie folgt:

- Notendifferenz = Note der Heimteam - Note der Auswärtsteam, vor dem Spieltag
- Tordifferenz = Tore (von der Heimmannschaft) - Gegentore, vom Spiel

<figure style="text-align: center">
  <img src="/plots/fussball_denken.png" alt="A person thinking about football" />
  <figcaption>Ein Fachmann denkt über Fußball. Bild von DALL-E 3.</figcaption>
</figure>

## Lineare Regression

Lineare Regression ist ein einfaches Modell, das Daten mit einer linearen Funktion prognostiziert.
Das bedeutet, dass die Funktion eine Summe von Koeffizient mal Variable ist.
In diesem Modell ist die Notendifferenz die eigene eingebene Variable.
Die ausgebene Variable ist die Tordifferenz.
Dafür sind unsere Datenpunkte (Notendifferenz, Tordifferenz) für jedes Spiel in der 1. Bundesliga.

Die einige Koeffizient in diesem Modell sagt uns, wie viele Notenpunkte eine Tordifferenz macht.
Zum Beispiel, wenn der Koeffizient -,5 ist, prognostiziert dieses Modell +1 in der Tordifferenz bei jeder weiteren -2 Notendifferenz.

<figure style="text-align: center">
  <img src="/plots/note_lin_reg.png"/>
  <figcaption>Lineare Regression über Notendifferenz gegen Tordifferenz</figcaption>
</figure>

## Resultaten

Dieses Modell bekommt 268 Punkte im Tippspiel und liegt auf Platz 6.
Sehr Erfolgreiche für ein einfaches Modell!

<table border="1" class="dataframe rendered_html" align="center">
  <thead>
    <tr style="text-align: left;">
      <th></th>
      <th>Team</th>
      <th>Points</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Bayer 04 Leverkusen</td>
      <td>287</td>
    </tr>
    <tr>
      <th>1</th>
      <td>FC Augsburg</td>
      <td>285</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Hertha BSC Berlin</td>
      <td>285</td>
    </tr>
    <tr>
      <th>3</th>
      <td>VfL Woflsburg</td>
      <td>274</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Bayern München</td>
      <td>271</td>
    </tr>
    <tr>
      <th>5</th>
      <td>SC Freiburg</td>
      <td>270</td>
    </tr>
    <tr style="background: orange">
      <th></th>
      <td>Fragen die Fachleute</td>
      <td>268</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Eintracht Frankfurt</td>
      <td>266</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Borussia Mönchengladbach</td>
      <td>261</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1. FC Heidenheim</td>
      <td>256</td>
    </tr>
    <tr>
      <th>9</th>
      <td>1. FC Union Berlin</td>
      <td>246</td>
    </tr>
    <tr>
      <th>10</th>
      <td>VfL Bochum</td>
      <td>246</td>
    </tr>
    <tr>
      <th>11</th>
      <td>RB Leipzig <b>(ich)</b></td>
      <td>235</td>
    </tr>
    <tr>
      <th>12</th>
      <td>BVB Borussia Dortmund</td>
      <td>235</td>
    </tr>
    <tr>
      <th></th>
      <td>2:1 Heimsieg</td>
      <td>229</td>
    </tr>
    <tr>
      <th>13</th>
      <td>VfB Stuttgart</td>
      <td>219</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1. FC Köln</td>
      <td>209</td>
    </tr>
    <tr>
      <th></th>
      <td>1:1 Unentschieden</td>
      <td>190</td>
    </tr>
  </tbody>
</table>

## Schlussfolgerung

Dieses Modell ist noch relativ einfach und besser als unsere ersten Modellen -- die Fachleute kennen sich aus!
Können wir mit mehr Daten ein besseres Modell bauen?
Finden wir heraus!

<a href="{{ "/erste_modelle/" | relative_url }}" class="button" style="float: left;">
  <i class="fas fa-chevron-circle-left"></i>
  Erste Modelle
</a>

<a href="{{ "/linear_regression/" | relative_url }}" class="button" style="float: right;">
  <i class="fas fa-chevron-circle-right"></i>
  Kürzliche Leistungen
</a>