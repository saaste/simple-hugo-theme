# Simple Hugo Theme
Tämä on yksinkertainen [Hugo](https://gohugo.io)-teema, jonka avulla ensikertalainen voi tutustua Hugon perustoiminnallisuuksiin.

Olen poistanut teemasta ison osan ylimääräisestä tauhkasta, jonka Hugo oletuksena luo. Olen myös lisännyt sivupohjiin joitakin kommentteja, jotka toivon mukaan auttavat ymmärtämään, mitä mikäkin rivi tekee. Kommentit näyttävät tältä: `{{/* Tämä on kommentti */}}`

## Asentaminen
Asentaminen on helpointa, kun asetat teeman Git submoduleksi seuraavilla komennoilla:

```shell
git submodule add --depth=1 https://github.com/saaste/simple-hugo-theme.git themes/simple-hugo-theme
git submodule update --init --recursive
```

Mikäli sinun on myöhemmin päivitettävä teemaa, aja:

```shell
git submodule update --remote --merge
```