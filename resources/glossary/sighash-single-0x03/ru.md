---
term: SIGHASH_SINGLE (0X03)

---
Тип флага SigHash, используемый в подписях транзакций Bitcoin для указания того, что подпись применяется ко всем входам транзакции и только к одному выходу, соответствующему индексу одного и того же подписанного входа. Таким образом, каждый вход, подписанный `SIGHASH_SINGLE`, конкретно связан с определенным выходом. Остальные выходы не фиксируются подписью и могут быть изменены позже. Этот тип подписи полезен в сложных транзакциях, где участники хотят связать определенные входы с определенными выходами, оставляя при этом свободу действий для других выходов транзакции.