---
term: STONEWALL X2

---
A specific form of Bitcoin transaction aimed at increasing user privacy during a spend, by collaborating with a third party not involved in the expenditure. This method simulates a mini-coinjoin between two participants, while making a payment to a third party. Stonewall x2 transactions are available on both the Samourai Wallet app and the Sparrow Wallet software (both are interoperable).

Its operation is relatively simple: it uses a UTXO in our possession to make the payment and seeks the help of a third party who also contributes with a UTXO they own. The transaction ends with four outputs: two of them of equal amounts, one intended for the address of the payment recipient, the other to an address belonging to the collaborator. A third UTXO is sent back to another address of the collaborator, allowing them to recover the initial amount (a neutral action for them, minus the mining fees), and a last UTXO returns to an address we own, which constitutes the change from the payment. Thus, three different roles are defined in Stonewall x2 transactions:


- The sender, who makes the effective payment;
- The collaborator, who provides bitcoins to improve the overall anonymity of the transaction, while fully recovering their funds at the end;
- The recipient, who may be unaware of the specific nature of the transaction and simply awaits a payment from the sender.

![](../../dictionnaire/assets/3.webp)

The Stonewall x2 structure adds a lot of entropy to the transaction and muddles the tracks of chain analysis. From the outside, such a transaction can be interpreted as a small coinjoin between two people. But in reality, it's a payment. This method thus generates uncertainties in chain analysis, or even leads to false trails. Even if an external observer manages to identify the pattern of the Stonewall x2 transaction, they will not have all the information. They will not be able to determine which of the two UTXOs of equal amounts corresponds to the payment. Moreover, they will not be able to know who made the payment. Finally, they will not be able to determine if the two input UTXOs come from two different people or if they belong to a single person who merged them. This last point is due to the fact that classic Stonewall transactions follow exactly the same pattern as Stonewall x2 transactions. From the outside and without additional information on the context, it is impossible to differentiate a Stonewall transaction from a Stonewall x2 transaction. However, the former are not collaborative transactions, while the latter are. This adds even more doubt about the expenditure.