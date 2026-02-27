## Harjoitus 2

Kysymys: Tarkastele tekemiäsi talletuksia komennolla git log. Kokeile myös komentoa laajentimella --stat. Mitä lisätietoa saat?

V: git log --stat listaa talletukset ja --stat -laajennin lisää myös muutokset

## Harjoitus 3

Kysymys: Poista kaikki loput muutokset työtilasta. Mitä tapahtui uusille untracked-tilassa oleville tiedostoille?

V: Git reset (--hard) ei vaikuta untracked-tilassa oleviin tiedostoihin ollenkaan.

Kysymys: Tee useita muutoksia ja talleta ne.
Peruuta talletus komennolla revert.
Mitä näyttää komento log?

V: 

    commit 140ff9f680b3380fcac56914223c7d117a35fd46 (HEAD -> master)
    Author: JarnoRyhanen <jarno.ryhanen02@gmail.com>
    Date: Fri Feb 27 13:30:29 2026 +0200

    Revert "Lisätty data.csv, info.json ja README.md"

    This reverts commit cb63dbf437b6588b6cf34e2e4a2d5081b1b5c4c1.

    README.md | 11 -----------
    data.csv | 1 -
    info.json | 4 ----
    3 files changed, 16 deletions(-)


## Harjoitus 4

Kysyvys: Kokeile vaihtaa aktiivista haaraa haarojen master ja tyylit välillä ja lataa sivu selaimessa aina uudelleen. Miten sivu muuttuu?

V: Css-tyylit eivät näy master-haarassa, mutta näkyvät tyylit-haarassa.


Kysymys: Kokeile nyt vaihtaa aktiivista haaraa haarojen master ja tyylit välillä ja lataa sivu selaimessa aina uudelleen. Miten sivu muuttuu?

V: Tyylit ovat nyt molemmilla haaroilla samat mergen jälkeen.