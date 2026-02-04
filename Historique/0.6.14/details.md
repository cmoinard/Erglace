# Erglace 0.6.14

[Légende](../legend.md)

## Résumé

- tournante `X->W->J`
- tournante `Z->K`

## Disposition

```
base = '''
╭╌╌╌╌╌┰─────┬─────┬─────┬─────┬─────┰─────┬─────┬─────┬─────┬─────┰╌╌╌╌╌┬╌╌╌╌╌╮
┆ ~   ┃ € ‚ │ @   │ #   │ $   │ %   ┃ ^   │ &   │ *   │ «   │ »   ┃ _ – ┆ + ± ┆
┆ `   ┃ 1 „ │ 2 ° │ 3 ¶ │ 4 ¢ │ 5 ‰ ┃ 6   │ 7   │ 8 § │ 9 “ │ 0 ” ┃ / ÷ ┆ = ≠ ┆
╰╌╌╌╌╌╂─────┼─────┼─────┼─────┼─────╂─────┼─────┼─────┼─────┼─────╂╌╌╌╌╌┼╌╌╌╌╌┤
·     ┃ J   │ ! ¡ │ O   │ F   │ Z   ┃ Q   │ D   │ L   │ C   │ X   ┃ {   ┆ }   ┆
·     ┃     │***¨ │   ô |   è │     ┃     │   ù │   û │   ç │   ß ┃ [   ┆ ]   ┆
·     ┠─────┼─────┼─────┼─────┼─────╂─────┼─────┼─────┼─────┼─────╂╌╌╌╌╌┼╌╌╌╌╌┤
·     ┃ A   │ I   │ E   │ U   │ ;   ┃ G   │ T   │ N   │ S   │ R   ┃ "   ┆ |   ┆
·     ┃   œ │   æ │   ê │   é │ , _ ┃  *µ │   à │   â │   î │   y ┃ '   ┆ \   ┆
╭╌╌╌╌╌╂─────┼─────┼─────┼─────┼─────╂─────┼─────┼─────┼─────┼─────╂╌╌╌╌╌┴╌╌╌╌╌╯
┆ >   ┃ :   │ Y   │ ? ¿ │ H   │ K   ┃ B   │ P • │ M   │ V   │ W   ┃           ·
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

La version 0.6.13 est très bien, mais il reste encore quelques frictions.

`Y` en touche morte est très pratique, mais quand même un peu frusté de pas l’avoir à une meilleure place. J’ai réessayé de le mettre ailleurs, mais aucune solution n’est satisfaisante. L’inversion `y<->,` semble être la meilleure alternative, mais avec ça la répartition des doigts de la main droite en français est très mauvaise car l’annulaire devient plus utilisé que l’index. Tout autre place finit par tout casser et les stats explosent. Donc, je laisse Y en 3B avec touche morte. 

Pour la principale tournante, c’est un peu plus agréable.

`X` en 4H à gauche était vraiment pas terrible pour les enchaînements `aix`, `fix`, `ixe` ou `oix`. Je le passe donc à droite en 4H, ça simplifie ces enchaînements, c’est à proximité de `C` et `V` et ça fait quelques petits roulements intérieurs :
- `xc` (0.011% fr et 0.023% en)
- `xt` (0.010% fr et 0.015% en)
- `xp` (0.016% fr et 0.019% en), bien que celui-ci soit pas top car ciseau 4H-1B

`W` en 4H était pas très accessible, ce qui pose pas de problèmes en français, mais un peu plus galère en anglais. Passer `W` en 4B à droite est plus confortable en anglais, surtout pour les enchaînements suivants :
- `tw` (0.048%)
- `nw` (0.080%)
- `sw` (0.068%)
- `rw` (0.037%), donc SFU mais c’en était déjà un avant
- `lw` (0.016%), donc ciseau, mais peu fréquent

`K` est très peu utilisé en français, mais l’est pas mal en anglais :
- `ke` (0.255%)
- `ka` (0.138%)
- `ki` (0.129%)
- `ko` (0.083%)
- `ku` (0.015%)
Donc `K` doit rester en extension de l’index car peu combiné avec `u`. Mais l’avoir en 1HE oblige à bouger la main, alors que l’avoir en 1BE est bien plus confortable.

J’avais déjà testé `J` en 1HE, c’était correct mais moins pratique qu’en 4H ou 4B à droite. Les places à droite étant utilisées par des lettres plus pertinentes (`X` et `W`), il reste que des places à gauche :
- Métriques :
    - `je` (0.327% fr)
    - `jo` (0.102% fr, 0.025% en)
    - `j’` (0.077% fr)
    - `ju` (0.083% fr, 0.034% en)
    - `ja` (0.058% fr et 0.011% en)
    - `ji` (0.002% fr et en)

- Positionnement en 4B :
    - `je` et `ju` sont confort
    - `ja` en SFU
    - `j’` et `jo` en ciseaux inconfortables
- Positionnement en 3B :
    - `ju` confort
    - `je` à peu près confort (un peu bof sur un clavier standard sans angle-mod)
    - `jo` en gros ciseau
    - `j’` ciseau/SFU
    - `ja` en mini-ciseau pas terrible
- Positionnement en 4H :
    - `jo` et `ju` sont confort
    - `jou` devient un roulement agréable, d’autant plus qu’il est plus courant que `joi` en français (anecdotique en anglais)
    - `j’` en roulement ok, petite danse pas si désagréable pour `j’ai`
    - `ja` en SFU
    - `je` en 4H-2 moyen pour le principal usage de `j`
- Positionnement en 1HE :
    - SFU pour `ju`
    - confort `ja`
    - extension ok pour `jo` et `j’`
    - `je` pas très confort
- Positionnement en 1BE :
    - SFU pour `ju`
    - confort pour `je` et `ja`
    - ciseaux pour `jo` et `j’` mais pas si inconfortable, à titre de comparaison `bl` se fait avec le même enchaînement que `jo` et a des fréquences plus élevées (0.178% fr, 0.118% en)

Donc la meilleure place est 1BE, mais elle est prise par le `K` qui en bénéficie davantage. 4B et 3B sont à proscrire tellement ça apporte plus de problèmes que de solutions. Reste 4H et 1HE.

`Z` est très peu utilisé en général (moins de 0.010%) sauf :
- `za` (0.017% fr, 0.034%), dû au fait que le corpus est Don Quichote, surreprésentation de `Panza`, le nom de Sancho
- `z,` (0.017% fr, 0.002%)
- `ze` (0.154% fr, 0.024%)
Deux options :
- 4H :
    - Pas de SFU (hormis la surreprésentation dûe au corpus particulier)
    - `z,` confort
    - `ez` ok
    - `uez` en roulement extérieur ok `1->2->4H`
    - `iez` en mauvaise redirection `3->2->4H`
- 1HE :
    - `iez` en roulement `3->2->1HE`
    - `ez` ok
    - `z,` en SFU mais faisable en faisant un glissé du haut vers le bas
    - `uez` en redirection `1->2->1HE`


Reste à trancher `J` et `Z`. À titre perso, j’ai une préférence pour `J` en 4H et `Z` en 1HE. Je suis avec cette configuration depuis plusieurs jours et c’est agréable, principalement pour :
- `iez` en roulement `3->2->1HE`
- `jo` et `ju` sont confort
- `jou` en roulement agréable
- `j’` en roulement ok, petite danse pas si désagréable pour `j’ai`