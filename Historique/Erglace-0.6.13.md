# Erglace 0.6.13

[Légende](_Legende.md)

## Résumé

- retour en arrière pour l’inversion `y` et `,`
- présence du `y` en touche morte pour faciliter les enchaînements

## Disposition

```
base = '''
╭╌╌╌╌╌┰─────┬─────┬─────┬─────┬─────┰─────┬─────┬─────┬─────┬─────┰╌╌╌╌╌┬╌╌╌╌╌╮
┆ ~   ┃ € ‚ │ @   │ #   │ $   │ %   ┃ ^   │ &   │ *   │ «   │ »   ┃ _ – ┆ + ± ┆
┆ `   ┃ 1 „ │ 2 ° │ 3 ¶ │ 4 ¢ │ 5 ‰ ┃ 6   │ 7   │ 8 § │ 9 “ │ 0 ” ┃ / ÷ ┆ = ≠ ┆
╰╌╌╌╌╌╂─────┼─────┼─────┼─────┼─────╂─────┼─────┼─────┼─────┼─────╂╌╌╌╌╌┼╌╌╌╌╌┤
·     ┃ X   │ ! ¡ │ O   │ F   │ K   ┃ Q   │ D   │ L   │ C   │ W   ┃ {   ┆ }   ┆
·     ┃     │***¨ │   ô |   è │     ┃     │   ù │   û │   ç │   ß ┃ [   ┆ ]   ┆
·     ┠─────┼─────┼─────┼─────┼─────╂─────┼─────┼─────┼─────┼─────╂╌╌╌╌╌┼╌╌╌╌╌┤
·     ┃ A   │ I   │ E   │ U   │ ;   ┃ G   │ T   │ N   │ S   │ R   ┃ "   ┆ |   ┆
·     ┃   œ │   æ │   ê │   é │ , _ ┃  *µ │   à │   â │   î │   y ┃ '   ┆ \   ┆
╭╌╌╌╌╌╂─────┼─────┼─────┼─────┼─────╂─────┼─────┼─────┼─────┼─────╂╌╌╌╌╌┴╌╌╌╌╌╯
┆ >   ┃ :   │ Y   │ ? ¿ │ H   │ Z   ┃ B   │ P • │ M   │ V   │ J   ┃           ·
┆ <   ┃ . … │     │ - ‑ │   – │   — ┃     │   · │   µ │   ñ │     ┃           ·
╰╌╌╌╌╌┸─────┴─────┴─────┴─────┴─────┸─────┴─────┴─────┴─────┴─────┚ · · · · · ·
'''


altgr = '''
╭╌╌╌╌╌┰─────┬─────┬─────┬─────┬─────┰─────┬─────┬─────┬─────┬─────┰╌╌╌╌╌┬╌╌╌╌╌╮
┆     ┃   ¹ │   ² │   ³ │   ⁴ │   ⁵ ┃   ⁶ │   ⁷ │   ⁸ │   ⁹ │   ⁰ ┃     ┆     ┆
┆     ┃   ₁ │   ₂ │   ₃ │   ₄ │   ₅ ┃   ₆ │   ₇ │   ₈ │   ₉ │   ₀ ┃     ┆     ┆
╰╌╌╌╌╌╂─────┼─────┼─────┼─────┼─────╂─────┼─────┼─────┼─────┼─────╂╌╌╌╌╌┼╌╌╌╌╌┤
·     ┃  *^ │   ≤ │   ≥ │  *¤ │   ‰ ┃  *˚ │     │   × │  *´ │  *` ┃     ┆     ┆
·     ┃   ^ │   < │   > │   $ │   % ┃   @ │   & │   * │   ' │   ` ┃     ┆     ┆
·     ┠─────┼─────┼─────┼─────┼─────╂─────┼─────┼─────┼─────┼─────╂╌╌╌╌╌┼╌╌╌╌╌┤
·     ┃  *ˇ │     │     │  *˙ │   ≠ ┃  */ │   ± │  *¯ │   ÷ │  *” ┃     ┆     ┆
·     ┃   { │   ( │   ) │   } │   = ┃   \ │   + │   - │   / │   " ┃     ┆     ┆
╭╌╌╌╌╌╂─────┼─────┼─────┼─────┼─────╂─────┼─────┼─────┼─────┼─────╂╌╌╌╌╌┴╌╌╌╌╌╯
┆     ┃  *~ │  *, │  *˛ │   – │     ┃   ¦ │   ¬ │  *¸ │   : │  *˘ ┃           ·
┆     ┃   ~ │   [ │   ] │   _ │   # ┃   | │   ! │   ; │   : │   ? ┃           ·
╰╌╌╌╌╌┸─────┴─────┴─────┴─────┴─────┸─────┴─────┴─────┴─────┴─────┚ · · · · · ·
'''

[spacebar]
shift       = "\u202f"  # NARROW NO-BREAK SPACE
altgr       = "\u0020"  # SPACE
altgr_shift = "\u00a0"  # NO-BREAK SPACE
1dk         = "\u2019"  # RIGHT SINGLE QUOTATION MARK
1dk_shift   = "\u2019"  # RIGHT SINGLE QUOTATION MARK
```

## Détails

En regardant les stats sur la tournante `y`-`,`, on a 3 options :
- A. `y` en 1E et `,` en 3B
- B. `,` en 1E et `y` en 3B
- C. `,` en 1E, `y` en 3B et touche morte

A est assez pratique notamment pour :
- `y` et `z` à proximité
- `,` et `.` à proximité et sur des doigts différents

B est ok, mais C devient beaucoup plus intéressant en termes de métriques. Je serai d’avis de prendre l’option C.

En termes d’usage, on a :
```
| Lettre | Fr       | En       |
| ,      |   2.004% |   1,990% |
| y      |   0,241% |   1,781% |
```

Et la table de combinaison :
```
| Digram | Fr       | En       | Total Fr | Total En |
| yu     |   0,000% |   0,000% |          |          |
| uy     |   0,031% |   0,002% |   0,031% |   0,002% |
| yi     |   0,000% |   0,039% |          |          |
| iy     |   0,000% |   0,000% |   0,000% |   0,039% |
| ye     |   0,075% |   0,060% |          |          |
| ey     |   0,001% |   0,200% |   0,076% |   0,261% |
| ya     |   0,057% |   0,010% |          |          |
| ay     |   0,041% |   0,259% |   0,098% |   0,268% |
| yo     |   0,004% |   0,232% |          |          |
| oy     |   0,066% |   0,020% |   0,070% |   0,252% |

| u,     |   0,038% |   0,017% |   0,038% |   0,017% |
| i,     |   0,115% |   0,006% |   0,115% |   0,006% |
| e,     |   0,632% |   0,376% |   0,632% |   0,376% |
| a,     |   0,037% |   0,050% |   0,037% |   0,050% |
| o,     |   0,065% |   0,112% |   0,065% |   0,112% |
```

`,` est autant utilisée en français et anglais, mais moyennement dans les 2 langues. Alors que `y` est tout autant utilisée en anglais mais très peu en français. Léger avantage pour l’option A.

Niveau stats, avantage aussi pour l’option A :
- La charge des doigts est meilleure, on décharge un peu 3 et on charge 1. Mais c’est surtout intéressant en français car dans l’option B, 3 est plus chargé que 1, ce qui est un problème.
- sfu équivalents bien que très légèrement plus bas
- mêmes ciseaux en fr, mais un peu plus élevés en anglais

Mais si dans l’option A on remet `y` en touche morte, en plus de l’avoir en 3B, les stats vont largement en faveur de l’option A :
- Meilleure charge des doigts
- Meilleure latéralisation
- SFU plus bas, surtout en anglais (on passe de 1.05% à 0.95%)
- Moins de ciseaux (1.29% à 1.09% en fr, 2.11% à 1.85% en anglais)
- Moins d’extensions en anglais, mais plus en français