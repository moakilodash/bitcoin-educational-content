---
term: BECH32 И BECH32M

---
`Bech32` и `Bech32m` - два формата кодировки адресов для приема биткоинов. Они основаны на слегка модифицированном основании 32. Они включают в себя контрольную сумму, основанную на алгоритме коррекции ошибок под названием BCH (*Bose-Chaudhuri-Hocquenghem*). По сравнению с адресами Legacy, закодированными в `Base58check`, адреса `Bech32` и `Bech32m` имеют более эффективную контрольную сумму, позволяющую обнаруживать и потенциально автоматически исправлять опечатки. Кроме того, их формат отличается лучшей читаемостью, поскольку содержит только строчные символы. Вот матрица сложения для этого формата по основанию 10:

&nbsp;

| + | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 |

| --- | --- | --- | --- | --- | --- | --- | --- | --- |

| 0 | q | p | z | r | y | 9 | x | 8 |

| 8 | g | f | 2 | t | v | d | w | 0 |

| 16 | s | 3 | j | n | 5 | 4 | k | h |

| 24 | c | e | 6 | m | u | a | 7 | l |

&nbsp;

Bech32 и Bech32m - форматы кодирования, используемые для представления адресов SegWit. Bech32 - это формат кодирования адресов, представленный BIP173 в 2017 году. В нем используется определенный набор символов, состоящий из цифр и строчных букв, чтобы минимизировать ошибки при наборе и облегчить чтение. Адреса Bech32 обычно начинаются с `bc1`, чтобы указать, что они являются родными для SegWit. Этот формат используется только для адресов SegWit V0, со скриптами P2WPKH (Pay to Witness Public Key Hash) и P2WSH (Pay to Witness Script Hash). Однако у формата Bech32 есть небольшой неожиданный недостаток. Если последним символом адреса является `p`, добавление или удаление любого количества символов `q`, непосредственно предшествующих ему, не приводит к аннулированию контрольной суммы. Это не влияет на существующее использование адресов SegWit V0 (BIP173) из-за их ограничения двумя определенными длинами. Однако это может повлиять на будущее использование кодировки Bech32. Формат Bech32m - это просто формат Bech32 с исправленной ошибкой. Он был введен в BIP350 в 2020 году. Адреса Bech32m также начинаются с `bc1`, но они специально разработаны для совместимости с SegWit V1 (Taproot) и более поздними версиями, со скриптом P2TR (Pay to TapRoot).