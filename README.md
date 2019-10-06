# Git på dansk

## Introduktion

Det danske omgangssprog for begreberne og kommandoerne i versionskontrolsystemet `git` er cirkussprog.
Man anvender enkle fordanskninger af de engelske begreber, som f x _"Kan du pushe branchen?"_ eller _"Jeg puller!"_.
Udtalen foregår typisk med anvendelse af amerikansk engelsk med stærk østdansk accent.
Sig derfor /bwæːnɕ/, ikke /bɹɑːntʃ/.

Dette dokument forsøger at etablere en ren dansk fagjargon, som kan anvendes ikke mindst i skriftlig fremstilling.
Det er underforstået, at kommunikation i kampens hede blandt udviklere bedst foregår på cirkussprog.
Man skal desuden være opmærksom på, at man ved anvendelse af dansk terminologi kan udsætte sig for et betydeligt tab af social status blandt fagfæller.

## Forslag


| Udsagnsord  | Nuværende brug | Forslag       |
|-------------|----------------|---------------|
| pull        | pulle          | hive          |
| push        | pushe          | puffe         |
| fetch       | fetche         | hente         |
| branch      | branche        | forgrene      |
| commit      | committe       | fastlægge     |
| rebase      | rebase         | ompode        |
| merge       | merge          | flette        |
| squash      | squashe        | mose          |
| stash       | stashe         | gemme         |
| tag         | tagge          | markere       |
| cherry-pick | cherry-picke   | håndplukke    |
| amend       | amende         | hovsarette    |
| blame       | blame          | klandre       |
| bisect      | bisecte        | indkredse     |
| clone       | clone/klone    | klone         |

| Navneord     | Nuværende brug | Forslag      |
|--------------|----------------|--------------|
| repository   | repository     | repositorium, repo |
| branch       | branch         | gren         |
| commit       | commit         | fastlæggelse |
| pull request | pull request   | hiveanmodning|
| stash        | stash          | gemme        |
| tag          | tag            | mærkning     |

## Eksempler

    - Gider i hive fra den gren, jeg lige har ompodet og puffet til GitHub?

    - Jeg har lige forgrenet og har fastlagt ændringerne fra mit gemme der.

    - Send lige en hiveanmodning, når du er færdig med fletningen!

    - Det håndplukker vi da bare fra udviklergrenen.
    
    - Hov, jeg tvangspuffede vistnok til hovedgrenen!

    - Husk at mose dine fastlæggelser, inden du fletter.

## Dagligt brug

Nedenunder er der en række kommandoer til at få konfigureret git til et dansk
udviklingsmiljø. Desværre er man nødsaget til at bruge ae/oe/aa i stedet for
æ/ø/ø pga. en fejl i git (overvej at rette det og sende en hiveanmodning til
git-vedligeholderen!). Følgende kommandoer ændrer din `~/.gitconfig` og har
global effekt.

    git config --global alias.hiv pull
    git config --global alias.puf push
    git config --global alias.gren branch
    git config --global alias.forgrena branch
    git config --global alias.fastlaeg commit
    git config --global alias.ompod rebase
    git config --global alias.flet merge
    git config --global alias.sammenflet merge
    git config --global alias.gem stash
    git config --global alias.klandr blame
    git config --global alias.marker tag
    git config --global alias.maerke tag
    git config --global alias.indkreds bisect
    git config --global alias.klon clone
