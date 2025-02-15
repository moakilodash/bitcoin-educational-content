---
term: WITNESSSCRIPT

---
一个脚本，用于指定可以从 P2WSH 或 P2SH-P2WSH UTXOs 支出比特币的条件。通常，"见证脚本 "决定了 SegWit 标准下多重签名钱包的条件。在这些脚本标准中，UTXO（输出）的`scriptPubKey`包含`见证脚本`的哈希值。要将该UTXO作为新交易的输入，持有者必须披露原始 "见证脚本"，以证明其与 "脚本发布密钥 "中的指纹匹配。然后，"见证脚本 "必须包含在交易的 "脚本见证 "中，其中还包含验证脚本所需的元素，如签名。因此，对于 SegWit 来说，"见证脚本 "等同于 P2SH 交易中的 "赎回脚本"，不同之处在于它被放在交易见证中，而不是放在 "脚本签名 "中。

> ► *注意，"见证脚本 "不应与 "脚本见证 "混淆。虽然 `witnessScript` 定义了 P2WSH 或 P2SH-P2WSH UTXO 的支出条件，其本身就构成了一个脚本，但 `scriptWitness` 包含了任何 SegWit 输入的见证数据*。