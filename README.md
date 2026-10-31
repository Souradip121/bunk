# Bunk calculator

How many classes can you skip and still sit at 75%? Or, if you're below it, how many do you have to attend in a row to get back?

**Use it:** https://souradip121.github.io/bunk/

Type classes attended and classes held (and your college's minimum if it isn't 75%). With *a* attended out of *t* held and a minimum of *m*%:

- classes you can still skip = ⌊(100a − m·t) / m⌋ (at 75%: ⌊(4a − 3t) / 3⌋)
- classes to attend in a row to get back = ⌈(m·t − 100a) / (100 − m)⌉ (at 75%: ⌈3t − 4a⌉)

36 of 40 → skip 8 (36/48 = 75%). 25 of 40 → attend 20 in a row (45/60 = 75%).

One HTML file, no backend, no login: your numbers stay on your phone. Shareable links work too: `?a=36&t=40&m=75`.

Made by [@souradip.sh](https://www.instagram.com/souradip.sh/). Use it responsibly. Or don't.
