# Chess
## Schritt 1: Spielfeld
- 8x8 bestzbare Felder (zweidimensionales array?)
### Feld
- schwarz/weiß (als non-nullable bool)
- besetzt/unbesetzt (als non-nullable bool)
- Figureninhalt: welche Figur steht auf dem Feld?

ToString:
  - wenn unbesetzt: Farbe verwenden
  - wenn besetzt: Figurensymbol verwenden

### ToString-methode:
Leeres Feld:
```
  A   B   C   D   E   F   G   H
+---+---+---+---+---+---+---+---+
| # |   | # |   | # |   | # |   |  1
+---+---+---+---+---+---+---+---+
|   | # |   | # |   | # |   | # |  2
+---+---+---+---+---+---+---+---+
| # |   | # |   | # |   | # |   |  3
+---+---+---+---+---+---+---+---+
|   | # |   | # |   | # |   | # |  4
+---+---+---+---+---+---+---+---+
| # |   | # |   | # |   | # |   |  5
+---+---+---+---+---+---+---+---+
|   | # |   | # |   | # |   | # |  6
+---+---+---+---+---+---+---+---+
| # |   | # |   | # |   | # |   |  7
+---+---+---+---+---+---+---+---+
|   | # |   | # |   | # |   | # |  8
+---+---+---+---+---+---+---+---+
```
bei Initialisierung:
```
  A   B   C   D   E   F   G   H
+---+---+---+---+---+---+---+---+
| T | P | L | K | Q | L | P | T |  1
+---+---+---+---+---+---+---+---+
| B | B | B | B | B | B | B | B |  2
+---+---+---+---+---+---+---+---+
| # |   | # |   | # |   | # |   |  3
+---+---+---+---+---+---+---+---+
|   | # |   | # |   | # |   | # |  4
+---+---+---+---+---+---+---+---+
| # |   | # |   | # |   | # |   |  5
+---+---+---+---+---+---+---+---+
|   | # |   | # |   | # |   | # |  6
+---+---+---+---+---+---+---+---+
| b | b | b | b | b | b | b | b |  7
+---+---+---+---+---+---+---+---+
| t | p | l | q | k | l | p | t |  8
+---+---+---+---+---+---+---+---+
```
## Schritt 2: Figuren
Typ Figur: 
- weiß/schwarz
- Schachposition (AKA Welche Figur ist es eigentlich?)
