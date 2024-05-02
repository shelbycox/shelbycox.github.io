---
layout: page
title: "Erste Modelle"
class: home
mathjax: true
---

# Erste Modelle

## Eine einfache Vergehenweise

Ein einfaches Modell tippt immer den gleichen Spielstand.
Zum Beispiel, man kann immer einen 1:1 Unentschieden oder einen 1:0 Heimsieg tippen.
Meine erste Modelle folgen diese Vorgehenweise.

Ein Vorteil von dieser Vorgehenweise ist, dass es sehr wenig Information braucht. 
Wir konnen den Spielstand aus den häufstigen Spielstände, die unter sind, auswählen.

<img src="/plots/heatmap_counts.png" alt="Heatmap von 1. Bundesliga Spielstandzahlen" />

<img src="/plots/heatmap_percent.png" alt="Heatmap von 1. Bundesliga Spielstandprozenten" />

## Resultaten

<div class="columns" markdown="1">

<div class="intro" markdown="1">

**Immer 1:1 Unentschieden**

Das 1:1 Unentschieden ist in den 1. Bundesliga Speilständen am häufigsten.
Ein Nachteil von diesem Spielstand ist, dass unentschidene Tipps, die nicht ganz richtig sind, in unserem Spiel nur 4 Punkte und nicht 5 Punkte bekommen.

Leider funkioniert dieses Modell ganz schlecht und nach dem 30. Spieltag liegt er an der letzten Stelle mit 190 Punkte.

</div>

<div class="intro" markdown="1">

**Immer 2:1 Heimsieg**

Der 2:1 Heimsieg ist in den 1. Bundesliga Spielstände am zweithäufigsten.
Der 2:1 Heimsieg ist nicht so häufig wie das 1:1 Unentschieden, aber man kann bei den 1:0, 3:2, 4:3, usw. Heimsiegen 5 Punkte bekommen.

Dieses Modell funktioniert ein bisschen besser mit 229 Punkten.
Nach dem 30. Spieltag liegt dieses Modelle an der 13. Stelle -- besser als zwei Personnen!

</div>

</div>

<div class="columns" markdown="1">

<table border="1" class="dataframe rendered_html" align="center">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Team</th>
      <th>Points</th>
    </tr>
  </thead>
  <tbody>
    <!-- <tr>
      <th></th>
      <td>Kürzliche Leistungen</td>
      <td>402</td>
    </tr> -->
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
    <!-- <tr>
      <th></th>
      <td>Fragen die Fachleute</td>
      <td>268</td>
    </tr> -->
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
    <tr style="background: orange">
      <th></th>
      <td>2:1 Heimsieg</td>
      <td>229</td>
    </tr>
    <tr>
      <th>15</th>
      <td>VfB Stuttgart</td>
      <td>227</td>
    </tr>
    <tr style="background: orange">
      <th></th>
      <td>1:1 Unentschieden</td>
      <td>204</td>
    </tr>
  </tbody>
</table>

</div>

## Schlussfolgerung

Dieses Modell ist einfach aber nicht so gut.
Es ist nicht so liecht den Tippspiel zu gewinnen!


<a href="{{ "/bundesliga" | relative_url }}" class="button" style="float: left;">
  <i class="fas fa-chevron-circle-left"></i>
  Einleitung
</a>

<a href="{{ "/experte" | relative_url }}" class="button" style="float: right;">
  <i class="fas fa-chevron-circle-right"></i>
  Fragen die Fachleute
</a>