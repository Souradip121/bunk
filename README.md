# bunk

How many classes can you still skip in every subject, and still sit at your college's minimum? Or, if you're below it, how many do you have to attend in a row to get back?

**Use it:** https://souradip121.github.io/bunk/

- Every subject at once, each with its verdict: **SKIP 8**, **ATTEND 12**, or **ON THE LINE**.
- 75%, 80% or 85% minimum, or any other number.
- One tap a day: **Present today** or **Bunked today**.
- **What a bunk costs:** your annual fees ÷ (classes a week × academic weeks) = what one lecture costs, and what your safe bunks are worth.

## The maths

With *a* classes attended out of *t* held and a minimum of *m*%:

- classes you can still skip = ⌊(100a − m·t) / m⌋ (at 75%: ⌊(4a − 3t) / 3⌋)
- classes to attend in a row to get back = ⌈(m·t − 100a) / (100 − m)⌉ (at 75%: ⌈3t − 4a⌉)

36 of 40 → skip 8 (36/48 = 75%). 27 of 40 → attend 12 in a row (39/52 = 75%). Percentages are floored to one decimal, so the app never rounds you up past the line.

The register on each subject's page shows your real counts. The order of the absences is made up, because the app doesn't know your dates.

## Links

- `?demo` shows the example (DBMS 36/40, Maths 27/40, OS 30/38) without touching what your phone saved.
- `?a=36&t=40&m=75` opens one subject from a shared link (the v1 format still works).
- The first version is kept at [/v1/](https://souradip121.github.io/bunk/v1/).

## How it's built

One HTML file, no backend, no login, no build step. Your numbers stay in your browser (localStorage). To host your own copy, fork this repo and turn on GitHub Pages for the `gh-pages` branch.

Made by [@souradip.sh](https://www.instagram.com/souradip.sh/). Use it responsibly. Or don't.

Fonts: Libre Caslon Text, Libre Caslon Display and Kalam, under the SIL Open Font License. v1 uses Oswald, Courier Prime and Archivo Black (also OFL).
