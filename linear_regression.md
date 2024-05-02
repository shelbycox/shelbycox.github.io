---
layout: page
title: "Kürzliche Daten"
class: home
mathjax: true
---

# Lineare Regression von kürzlichen Daten

Unsere letzte Modell ist eine lineare Regression über die kurzliche Leistungen von jede Mannschaft.

## Zentrale Daten

Nach diesem <a href="https://arxiv.org/pdf/2309.14807">Artikel</a> sind die letzen 5 Spiele am wichitgsten.
Der Stärke von einer Mannschaft kommt von diesen folgenden Sachen
- **Angriffskraft**: Tore, die in den letzten 5 Spielen geschossen sind.
- **Abwehrskraft**: Gegentore, die in den letztne 5 Spielen geschossen sind.
- **Gegnerskraft**: durchschnittliche Tordifferenz von letzten 5 Spielen des Gegners.
- **Heimvorteil**: +1 für die Heimmannschaft, -1 für den Auswärtsmannschaft.

Ich habe hier *nur Spiele in der 1. Bundesliga* benutzt (und kein Pokalspiele).

Zum Beispiel, im 32. Spieltag der Saison 2023/2024 hat der RB Leipzig die folgenden Daten:
- **Angriffskraft**: (4, 2, 3, 4, 0)
- **Abwehrskraft**: (1, 1, 0, 1, 0)
- **Gegnerskraft**: (.8, -.2, -1, .4, -1)
- **Heimvorteil**: (1, -1, 1, -1, 1)

Sein nächstes Spiel ist gegen die TSG Hoffenheim.

Von dieser lineare Regression bekommt man ein Tordifferenz.
Die Gesamttorezahl ist der Durchschnitt von alle Tore in den letzten fünf Spielen von beide Mannschaft, oder 0, wenn die frühere Zahl unter 0 ist.
Die Gegentorzahl ist hälfte der prognostizierte Gesamttorezahl.
Die Torzahl von der Heimmannschaft ist die Gegentorezahl plus das prognostizierte Tordifferenz.

Zum Beispiel, in den letzten 5 Spielen vom RB Leipzig gab es 13 Tore und 3 Gegentore. 
In den letzten 5 Spielen von der TSG Hoffenheim gab es 24 Tore und Gegentore.
Also dieses Modell tippt $(16 + 24)/20 = 2$ Gesamttore.
Der Tordifferenztipp ist $-2$, dafür tippt dieses Modell für Heimtore $1$ und für Gegentore $3$.

## Resultaten

<table border="1" class="dataframe rendered_html" align="center">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Team</th>
      <th>Points</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: orange">
      <th></th>
      <td>Kürzliche Leistungen</td>
      <td>402</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Hertha BSC Berlin</td>
      <td>305</td>
    </tr>
    <tr>
      <th>2</th>
      <td>VfL Woflsburg</td>
      <td>304</td>
    </tr>
    <tr>
      <th>3</th>
      <td>FC Augsburg</td>
      <td>302</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Bayern München</td>
      <td>298</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Bayer 04 Leverkusen</td>
      <td>287</td>
    </tr>
    <tr>
      <th>6</th>
      <td>SC Freiburg</td>
      <td>287</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Eintracht Frankfurt</td>
      <td>284</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1. FC Heidenheim</td>
      <td>275</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Borussia Mönchengladbach</td>
      <td>274</td>
    </tr>
    <tr>
      <th></th>
      <td>Fragen die Fachleute</td>
      <td>268</td>
    </tr>
    <tr>
      <th>10</th>
      <td>1. FC Union Berlin</td>
      <td>262</td>
    </tr>
    <tr>
      <th>11</th>
      <td>RB Leipzig</td>
      <td>257</td>
    </tr>
    <tr>
      <th>12</th>
      <td>VfL Bochum</td>
      <td>254</td>
    </tr>
    <tr>
      <th>13</th>
      <td>BVB Borussia Dortmund</td>
      <td>243</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1. FC Köln</td>
      <td>238</td>
    </tr>
    <tr>
      <th></th>
      <td>2:1 Heimsieg</td>
      <td>229</td>
    </tr>
    <tr>
      <th>15</th>
      <td>VfB Stuttgart</td>
      <td>227</td>
    </tr>
    <tr>
      <th></th>
      <td>1:1 Unentschieden</td>
      <td>204</td>
    </tr>
  </tbody>
</table>

## Schlussfolgerung

Dieses Modell ist toll! Im Durchschnitt bekam es $3,19$ Punkte pro Tipp und es gewann das Tippspiel mit 402 Punkte.

<a href="{{ "/experte" | relative_url }}" class="button" style="float: left;">
  <i class="fas fa-chevron-circle-left"></i>
  Fragen die Fachleute
</a>

<a href="{{ "/ende" | relative_url }}" class="button" style="float: right;">
  <i class="fas fa-chevron-circle-right"></i>
  Weitere Ideen
</a>