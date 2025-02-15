---
term: BIP11

---
BIP 由 Gavin Andresen 于 2012 年 3 月提出，提出了一种在比特币上创建多重签名交易的标准方法。该提案旨在通过要求多重签名来验证交易，从而提高比特币的安全性。BIP11 引入了一种新的脚本类型，命名为 "M-of-N multisig"，其中 `M` 代表从 `N` 个潜在公钥中所需签名的最小数量。该标准使用了比特币中已有的 "OP_CHECKMULTISIG "操作码，但该操作码之前并不符合节点的标准化规则。虽然这类脚本不再常用于实际的多位钱包，而是更倾向于 P2SH 或 P2WSH，但其使用仍然是可能的。它主要用于元协议，如 Stamps。不过，节点可以使用参数 `permitbaremultisig=0`，选择不转发这些 P2MS 交易。

> ► *如今，这一标准被称为 "裸多数据格 "或 "P2MS"。