# NEO24-Hevesi LSC – meccsek és tabellák

A klub összes csapatának menetrendje, eredményei és tabellái egy oldalon – a futsal-bajnokságokkal együtt.

- **Honlap:** `index.html` – a `data/klub.json` fájlból dolgozik.
- **Adatok:** `scripts/build.py` tölti le az MLSZ adatbankból (adatbank.mlsz.hu).
- **Futsal:** a futsal-csapatokat a `build.py` magától keresi meg a klub adatbank-oldalán (Futsal … versenyek, a klub minden csapata, pl. I. és II.). Az újonnan kiírt futsal-bajnokságok így külön beállítás nélkül bekerülnek. Kódjuk FU13, FU13B (II. csapat), FU15 stb.; a Csapatomban az U13, U15 … korosztályhoz tartoznak, 4+1-es felállással.
- **Frissítés:** a `.github/workflows/frissites.yml` kétnaponta lefut, frissíti az adatokat és újra közzéteszi az oldalt. Kézzel is indítható: **Actions → Frissítés és közzététel → Run workflow**.

A tabellák a lejátszott meccsek eredményeiből számoltak (győzelem 3, döntetlen 1 pont; holtversenyben gólkülönbség, majd több rúgott gól), levont pontokat és zöld asztalos döntéseket nem tartalmaznak.
