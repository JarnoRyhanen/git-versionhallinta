## Harjoitus 1

Ei kysymyksiä

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

## Harjoitus 5

Kysymys: Lisää GitHubiin tyhjä repositorio. Mitä GitHub-repositoriosivulla näkyy?

V: Sivulla näkyy ohjeet repositorioiden luontiin komentoriviltä.

Kysymys: Mitä GitHub-repositoriosivulla nyt näkyy? Mitä haaroja näet GitHubissa, entä paikallisessa repositoriossasi?

V: Paikallisella repolla näkyy haarat: 
        
        * master
        tyylit
        remotes/origin/master

Ja etärepossa vain haara master.

Kysymys: Etärepositoriossa on nyt eri sisältö kuin paikallisessa repositoriossasi. Hae muutokset paikalliseen repositorioon ja mene katsomaan niitä. Mikä muuttui?

V: 

    git checkout origin/master
    Note: switching to 'origin/master'.

    You are in 'detached HEAD' state. You can look around, make experimental
    changes and commit them, and you can discard any commits you make in this
    state without impacting any branches by switching back to a branch.

    If you want to create a new branch to retain commits you create, you may
    do so (now or later) by using -c with the switch command. Example:

    git switch -c <new-branch-name>

    Or undo this operation with:

    git switch -

    Turn off this advice by setting config variable advice.detachedHead to false

    HEAD is now at 163c94a Luotu uusi tiedosto Githubin kautta
    M       README.md


Kysymys: Palaa master-haaraan. Mitä komento status sanoo?

V: 

    git status   
    On branch master
    Your branch is behind 'origin/master' by 1 commit, and can be fast-forwarded.
    (use "git pull" to update your local branch)

    Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
            modified:   README.md

    no changes added to commit (use "git add" and/or "git commit -a")


Kysymys: Yhdistä origin/master-haaran muutokset. Mitä komento status nyt sanoo?

V:

	 git status
	 On branch master
	 Your branch is ahead of 'origin/master' by 1 commit.
  	 (use "git push" to publish your local commits)

	 nothing to commit, working tree clean

## Harjoitus 6

Ei kysymyksiä

## Harjoitus 7

Ei kysymyksiä