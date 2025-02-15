---
term: РАСПИЛЕННЫЙ УЗЕЛ

---
Обрезанный узел, по-английски "Pruned Node", - это полный узел, который выполняет обрезку блокчейна. Она заключается в постепенном удалении самых старых блоков после их надлежащей проверки, чтобы сохранить только самые последние блоки. Предел хранения задается в файле `bitcoin.conf` с помощью параметра `prune=n`, где `n` - максимальный размер блоков в мегабайтах (МБ). Если после этого параметра указано `0`, то обрезка отключается, и узел сохраняет блокчейн полностью.

Обрезанные узлы иногда рассматриваются как типы узлов, отличные от полных узлов. Использование обрезанных узлов может быть особенно интересным для пользователей, сталкивающихся с нехваткой места для хранения данных. В настоящее время полный узел должен иметь почти 600 ГБ только для хранения блокчейна. Обрезанный узел может ограничить требуемое хранилище до 550 МБ. Хотя обрезанный узел использует меньше дискового пространства, он поддерживает уровень проверки и подтверждения, аналогичный полному узлу. Поэтому обрезанные узлы предоставляют пользователям больше доверия по сравнению с легкими узлами (SPV).