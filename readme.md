# GIT-harjoittelua

Aluksi tehdään vähän harjoittelua pelkällä komentorivillä. Idea on, että aina kun tulee uusi idea tai toiminto mieleen, tehdään sille uusi branch. Tämä onnistuu komentorivillä

```bash
git checkout -b uusi-branch
```

Muutokset kyseiseen ominaisuuteen tehdään tässä branchissa, ei muualla. Committeja voi lisätä normaalisti ja ne näkyvät vain tässä branchissa. Jos vaihtaa branchia esimerkiksi takaisin master-branchiin, ei tiedostojärjestelmä näe uusia tiedostoja tai hakemistoja tai muutoksia vanhoihin tiedostoihin.

Kun muutokset on saatu valmiiksi ja uuden branchin sisältämä koodi toimii varmasti, voidaan se liittää takaisin master-branchiin. Ensin pitää kuitenkin siirtyä takaisin master-branchiin.

```bash
git checkout master
```

Nyt toisen branchin sisältämät muutokset voidaan yhdistää vanhan kanssa.

```bash
git merge uusi-branch --no-ff
```

Viimeiseksi pushataan muutokset Githubiin.

```bash
git push
```

HUOM! Tällä tavalla uudet branchit eivät näy Githubissa!
