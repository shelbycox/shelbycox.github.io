---
layout: page
title: "Ende"
class: home
mathjax: true
---

Unter diskutierte ich die Resultaten von den Modellen und Ideen für zukünftige Modellen.

# Resultaten

Das letzte Modell gewann das Tippspiel! Dafür ist diese Projekt ein großer Erfolg.

<table border="1" class="dataframe rendered_html" align="center">
  <thead>
    <tr style="text-align: left;">
      <th></th>
      <th>Team</th>
      <th>Points</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: orange">
      <th></th>
      <td>Kürzliche Leistungen</td>
      <td>687</td>
    </tr>
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
    <tr>
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

# Weitere Ideen

Können wir das Modell noch weiter verbessern? Hier sind ein paar Ideen.

### Verletzungen, Sperren, usw.
Was für einen Einflüss hat der zentrale Spieler?
Zum Beispiel, Orban und Klostermann, die Innenverteidiger beim RB Leipzig sind, haben Verletzungen in dieser Saison bekommen.
Was für einen Einflüss hat diese Verletzungen in der Abwehrkraft des RB Leipzig?
Ein neues Modell könnte auch Abwesenheiten verbinden.

### Motivationen
Mannschaften spielen vielleicht besser, wenn sie aufsteigen oder nicht absteigen wollen.
Zum Beispiel, nach dem 26. Spieltag liegt der 1. FSV Mainz 05 auf Platz 16 in der Tabelle and liegt der RB Leipzig auf Platz 5 in der Tabelle.
Nach dem Plätzedifferenz denkt man, dass der RB Leipzig gewinnen wird.
Aber der 1. FSV Mainz 05 gefühlte sich sehr motiviert, weil er auf Platz 15. liegt und nicht absteigen wollte.

Das Ergebnis? 0:0 Unentschieden.
Also, wir fragen: beinflüsst die Motivation von der Mannschaft das Ergebnis?
Und auch, wie können wir *Motivation* mit Zahlen beschreiben?

# Referenzen

Ich benutzte diese <a href="https://github.com/thomascamminady/AllBundesligaGamesEver?tab=License-1-ov-file">Software</a> um die Daten zu bekommen. Alle von den Daten hier kommt aus <a href="kicker.de">kicker.de</a>.

<a href="{{ "/linear_regression" | relative_url }}" class="button" style="float: left;">
  <i class="fas fa-chevron-circle-left"></i>
  Kürzliche Leistungen
</a>