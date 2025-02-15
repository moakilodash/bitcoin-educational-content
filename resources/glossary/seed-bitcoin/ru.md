---
term: SEED (BITCOIN)

---
В контексте Биткойна seed - это 512-битное значение, используемое для получения всех закрытых и открытых ключей, связанных с кошельком HD (Hierarchical Deterministic). Технически семя отличается от фразы (или мнемоники) восстановления. Фраза, которая обычно состоит из 12 или 24 слов, генерируется псевдослучайным образом из источника энтропии и завершается контрольной суммой. Эта фраза облегчает резервное копирование человеком, предоставляя текстовое представление значения, находящегося в основании кошелька.

Для получения фактического семени фраза восстановления, возможно, сопровождаемая дополнительной парольной фразой, обрабатывается алгоритмом PBKDF2 (*Password-Based Key Derivation Function 2*). В результате вычислений получается 512-битное семя. Именно это семя используется для детерминированной генерации мастер-ключа, а затем и всего набора ключей для кошелька HD в соответствии с BIP32.

![](../../dictionnaire/assets/31.webp)

> ► * Однако на обычном языке большинство биткойнеров, говоря о "семени", имеют в виду мнемоническую фразу, а не промежуточное состояние деривации, которое находится между мнемонической фразой и мастер-ключом.*