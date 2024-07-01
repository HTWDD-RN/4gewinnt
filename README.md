//Franz Regir - s86074, Radmir Mullagaliev - s85138

# 4gewinnt

PMC-Beleg---4-gewinnt
How-To:

Zwei Spieler setzen jeweils abwechselnd einen Punkt in die Matrix. Spieler 1 leuchtet immer, Spieler 2 blinkt.
Wenn ein Spieler dran ist, erscheint ein neuer (beständiger oder blinkender) Punkt auf der 8x8-Matrix. Dieser Punkt kann durch den linken und den rechten Button bewegt werden.
Wenn der bewegliche Punkt liegt, wo man ihn haben möchte, kann man den mittleren Button drücken, um die Eingabe zu bestätigen. Dadurch endet die Runde und der Gegenspieler ist dran.
Falls einer der Spieler 4 Punkte in einer Reihe hat (horizontal, vertikal oder diagonal), hat dieser gewonnen. Falls das Spielfeld voll wird, ohne dass dies eintritt, tritt ein Unentschieden auf.
Grober Ablauf einer Runde:

Punkte von Spieler 1 werden gesetzt. LCD gibt an, welcher Spieler dran ist und gibt kurze Instruktionen zu den Buttons.
Spieler kann den zu setzenden Punkt nach links und rechts bewegen. Dieser Loop wird gebrochen, sobald die Position des Punktes durch die mittlere Taste bestätigt wird. Währenddessen blinken die Punkte von Spieler 2.
Der Punkt wird gesetzt. Es wird geprüft, ob jemand gewonnen hat oder ein Unentschieden eingetreten ist. Falls ja: LCD gibt das Ergebnis an (Sieger oder Unentschieden) und bietet eine neue Runde an. Durch Druck des Mittleren Buttons (siehe LCD) wird das Spielfeld zurückgesetzt und ein neues Spiel beginnt. Falls nein: Der Spieler wechselt. Der andere Spieler ist nun am Zug und der Ablauf beginnt wieder in Schritt 1.
