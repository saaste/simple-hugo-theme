# Simple Hugo Theme
Tämä on yksinkertainen [Hugo](https://gohugo.io)-teema, jonka avulla ensikertalainen voi tutustua Hugon perustoiminnallisuuksiin.

Olen poistanut teemasta ison osan ylimääräisestä tauhkasta, jonka Hugo oletuksena luo. Olen myös lisännyt sivupohjiin joitakin kommentteja, jotka toivon mukaan auttavat ymmärtämään, mitä mikäkin rivi tekee. Kommentit näyttävät tältä: `{{/* Tämä on kommentti */}}`

## Asentaminen
Asentaminen on helpointa, kun asetat teeman Git submoduleksi seuraavilla komennoilla:

```shell
git submodule add --depth=1 https://github.com/saaste/simple-hugo-theme.git themes/simple-hugo-theme
git submodule update --init --recursive
```

Sinulla pitäisi nyt olla themes-hakemistossa alihakemisto, jonka nimi on simple-hugo-theme.

Ota teema käyttöön lisäämällä seuraava rivi Hugo-projektin juuressa olevaan `hugo.toml` asetustiedostoon:
```toml
theme = 'simple-hugo-theme'
```

Mikäli sinun on myöhemmin päivitettävä teemaa, aja:

```shell
git submodule update --remote --merge
```

## Virhetilanteet

### Teeman asennus antaa virheen: fatal: not a git repository (or any of the parent directories): .git

Tämä johtuu todennäköisesti siitä, ettei kotisivuprojektiasi ole alustettu Gitillä. Suorita seuraava komento ja yritä asentamista sen jälkeen uudelleen.

```shell
git init
```