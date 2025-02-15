---
name: Blockstream Green - рабочий стол
description: Использование Green Wallet на вашем компьютере
---
![cover](assets/cover.webp)

В этом уроке мы рассмотрим, как использовать программное обеспечение Blockstream Green на вашем компьютере для управления защищенным кошельком на аппаратном кошельке. При использовании аппаратного кошелька необходимо использовать программное обеспечение на вашем компьютере для управления кошельком. Это управляющее программное обеспечение не имеет доступа к приватным ключам; оно используется исключительно для ознакомления с балансом кошелька, генерации адресов получения, а также для создания и распространения транзакций, которые будут подписаны аппаратным кошельком. Green - это лишь одно из множества доступных решений для управления аппаратным кошельком Bitcoin.

В 2024 году Blockstream Green будет совместим только с устройствами Ledger Nano S (старая версия), Ledger Nano X, Trezor One, Trezor T и Blockstream Jade.

## Представляем блокчейн Green

Blockstream Green - это программное приложение, доступное на мобильных и настольных компьютерах. Ранее известный как Green Address, этот портфель стал проектом Blockstream после его приобретения в 2016 году.

Green - очень простое в использовании приложение, что делает его особенно подходящим для новичков. Оно предлагает различные функциональные возможности, такие как управление горячими кошельками, аппаратными кошельками, а также кошельками на сайдчейне Liquid. Вы также можете использовать его для создания кошелька только для часов.

![GREEN-DESKTOP](assets/fr/01.webp)

В этом руководстве мы сосредоточимся исключительно на использовании программы на компьютере. Чтобы узнать о других способах использования Green, обратитесь к другим нашим специализированным учебникам:

https://planb.network/tutorials/wallet/mobile/blockstream-green-e84edaa9-fb65-48c1-a357-8a5f27996143
https://planb.network/tutorials/wallet/mobile/blockstream-green-watch-only-66c3bc5a-5fa1-40ef-9998-6d6f7f2810fb
## Установка и настройка программного обеспечения Blockstream Green

Начните с установки программного обеспечения Blockstream Green на свой компьютер. Перейдите на [официальный сайт](https://blockstream.com/green/) и нажмите на кнопку "*Скачать сейчас*". Затем следуйте процессу установки в соответствии с вашей операционной системой.

![GREEN-DESKTOP](assets/fr/02.webp)

Запустите приложение, затем установите флажок "Я принимаю условия...*".

![GREEN-DESKTOP](assets/fr/03.webp)

Когда вы открываете Green в первый раз, на главном экране не будет настроенного портфолио. В дальнейшем, если вы будете создавать или импортировать портфели, они будут отображаться в этом интерфейсе. Прежде чем перейти к созданию портфолио, я рекомендую вам настроить параметры приложения под свои нужды. Нажмите на значок "Настройки" в левом нижнем углу.

![GREEN-DESKTOP](assets/fr/04.webp)

В меню "*Общие*" вы можете изменить язык программного обеспечения и активировать экспериментальные функции, если хотите.

![GREEN-DESKTOP](assets/fr/05.webp)

В меню "*Сеть*" вы можете включить подключение через Tor - сеть, которая шифрует все ваши соединения и делает вашу деятельность трудноотслеживаемой. Хотя эта опция может несколько замедлить работу приложения, она настоятельно рекомендуется для защиты вашей конфиденциальности, особенно если вы не используете собственный полноценный узел.

![GREEN-DESKTOP](assets/fr/06.webp)

Для пользователей, у которых есть собственный полноценный узел, Green предлагает возможность подключиться к нему через сервер Electrum, гарантируя полный контроль над информацией о сети Биткойн и распространением транзакций. Для этого нажмите на меню "*Кастомные серверы и валидация*", а затем введите данные своего сервера Electrum.

![GREEN-DESKTOP](assets/fr/07.webp)

Еще одна альтернативная функция - опция "*SPV Verification*", которая позволяет напрямую проверить определенные данные блокчейна и тем самым уменьшить необходимость доверять узлу Blockstream по умолчанию, хотя этот метод и не дает всех гарантий полноценного узла. Эту опцию также можно найти в меню "*Кастомные серверы и валидация*".

![GREEN-DESKTOP](assets/fr/08.webp)

После того как вы настроите эти параметры в соответствии с вашими потребностями, вы можете выйти из этого интерфейса.

## Импорт кошелька Bitcoin на Blockstream Green

Теперь вы готовы импортировать свой кошелек Bitcoin. Нажмите на кнопку "**Начать**".

![GREEN-DESKTOP](assets/fr/09.webp)

Вы можете выбрать между созданием локального программного кошелька и управлением холодным кошельком через аппаратный кошелек. В этом руководстве мы сосредоточимся на управлении аппаратным кошельком, поэтому вам нужно выбрать опцию "*На аппаратном кошельке*".

Опция "Только для просмотра*" позволяет импортировать расширенный открытый ключ (`xpub`) для просмотра операций портфеля без возможности расходовать связанные с ними средства.

![GREEN-DESKTOP](assets/fr/10.webp)

Если вы используете Jade, нажмите на соответствующую кнопку. В противном случае выберите "*Подключить другое аппаратное устройство*". В моем случае я использую Ledger Nano S. Для пользователей Ledger убедитесь, что вы установили приложение "*Bitcoin Legacy*" на свой аппаратный кошелек, так как Green поддерживает только эту версию.

![GREEN-DESKTOP](assets/fr/11.webp)

Подключите аппаратный кошелек к компьютеру и выберите Green.

![GREEN-DESKTOP](assets/fr/12.webp)

Дождитесь, пока Green импортирует информацию о вашем портфеле, после чего вы сможете получить к нему доступ.

![GREEN-DESKTOP](assets/fr/13.webp)

На этом этапе возможны два сценария. Если вы уже использовали свой аппаратный кошелек, вы должны увидеть, что ваша учетная запись появилась в программе. Но если вы, как и я, только что инициализировали свой аппаратный кошелек, сгенерировав мнемоническую фразу, но еще не использовали его, вам нужно будет создать учетную запись. Нажмите на кнопку "*Создать учетную запись*".

![GREEN-DESKTOP](assets/fr/14.webp)

Выберите "*Стандарт*", если вы хотите использовать классический кошелек.

![GREEN-DESKTOP](assets/fr/15.webp)

Теперь у вас есть доступ к вашей учетной записи.

![GREEN-DESKTOP](assets/fr/16.webp)

## Использование аппаратного кошелька с Blockstream Green

Теперь, когда ваш кошелек Bitcoin настроен, вы готовы получить свои первые саты! Просто нажмите на кнопку "*Получить*".

![GREEN-DESKTOP](assets/fr/17.webp)

Нажмите на кнопку "*Копировать адрес*", чтобы скопировать адрес, или отсканируйте его QR-код.

![GREEN-DESKTOP](assets/fr/18.webp)

Как только транзакция будет транслироваться в сети, она появится в вашем кошельке. Подождите, пока вы не получите достаточно подтверждений, чтобы считать транзакцию неизменной.

![GREEN-DESKTOP](assets/fr/19.webp)

Теперь, когда биткоины в вашем кошельке, вы готовы их отправить. Нажмите на кнопку "*Отправить*".

![GREEN-DESKTOP](assets/fr/20.webp)

На следующей странице введите адрес получателя. Вы можете ввести его вручную или отсканировать QR-код с помощью веб-камеры.

![GREEN-DESKTOP](assets/fr/21.webp)

Выберите сумму платежа.

![GREEN-DESKTOP](assets/fr/22.webp)

В нижней части экрана вы можете выбрать размер комиссии для данной операции. У вас есть выбор: следовать рекомендациям приложения или установить свою комиссию. Чем выше комиссия по отношению к другим ожидающим транзакциям, тем быстрее будет обработана ваша транзакция. Информацию о рынке комиссий можно найти на сайте [Mempool.space](https://mempool.space/) в разделе "*Транзакционные сборы*".

![GREEN-DESKTOP](assets/fr/23.webp)

Если вы хотите выбрать, какие именно UTXO будут использоваться в вашей транзакции, нажмите на кнопку "*Ручной выбор монет*".

![GREEN-DESKTOP](assets/fr/24.webp)

Проверьте параметры транзакции и, если все соответствует вашим ожиданиям, нажмите "*Следующее*".

![GREEN-DESKTOP](assets/fr/25.webp)

Дважды проверьте правильность адреса, суммы и расходов, затем нажмите "*Подтвердить транзакцию*".

![GREEN-DESKTOP](assets/fr/26.webp)

Убедитесь в правильности всех параметров транзакции на экране аппаратного кошелька, а затем подпишите транзакцию с его помощью.

![GREEN-DESKTOP](assets/fr/27.webp)

Как только транзакция будет подписана с аппаратного кошелька, Green автоматически транслирует ее в сеть Bitcoin. После этого транзакция появится на панели вашего кошелька Bitcoin и будет ожидать подтверждения.

![GREEN-DESKTOP](assets/fr/28.webp)

Теперь вы знаете, как легко настроить Blockstream Green для управления кошельком Bitcoin на аппаратном кошельке.

Если вы нашли этот урок полезным, я буду благодарен, если вы оставите свой отзыв о нем ниже. Не стесняйтесь поделиться этой статьей в своих социальных сетях. Большое спасибо!

Я также рекомендую вам ознакомиться с другим полным руководством по настройке горячего кошелька в мобильном приложении Blockstream Green:

https://planb.network/tutorials/wallet/mobile/blockstream-green-e84edaa9-fb65-48c1-a357-8a5f27996143