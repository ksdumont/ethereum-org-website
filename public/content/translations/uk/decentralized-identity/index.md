---
title: Децентралізована ідентичність
description: Що таке децентралізована ідентифікація і чому вона важлива?
lang: uk
template: use-cases
emoji: ":id:"
sidebarDepth: 2
image: /eth-gif-cat.png
summaryPoint1: Традиційні системи ідентифікації централізовано видають, підтримують і контролюють ваші ідентифікатори.
summaryPoint2: Децентралізована ідентифікація усуває залежність від централізованих третіх сторін.
summaryPoint3: Завдяки криптовалюті користувачі знову мають інструменти для видачі, зберігання та контролю власних ідентифікаторів і атестацій.
---

Сьогодні ідентифікація лежить в основі майже всіх аспектів вашого життя. Користування онлайн-сервісами, відкриття банківського рахунку, голосування на виборах, купівля нерухомості, працевлаштування — усе це потребує підтвердження особи.

Однак традиційні системи управління ідентифікацією вже давно покладаються на централізованих посередників, які видають, зберігають і контролюють ваші ідентифікатори та [атестації](#what-are-attestations). Це означає, що ви не можете контролювати інформацію, пов'язану з вашою особою, або вирішувати, хто має доступ до інформації, що ідентифікує особу (PII), і в якому обсязі ці особи мають доступ.

Для розв’язання цих проблем у нас є децентралізовані системи ідентифікації, побудовані на публічних блокчейнах, як-от Ethereum. Децентралізована ідентифікація дозволяє особам управляти інформацією, пов'язаною з їхньою ідентифікацією. Завдяки децентралізованим рішенням ідентифікації _ви_ можете створювати ідентифікатори, вимагати та зберігати свої атестації, не покладаючись на центральні органи, як-от постачальники послуг або уряди.

## Що таке ідентичність? {#what-is-identity}

Ідентичність — це особисте відчуття себе, що визначається унікальними характеристиками. Ідентичність означає бути _особою_, тобто окремою людською сутністю. Ідентичність може також стосуватися інших нелюдських суб'єктів, як-от організація або орган влади.

## Що таке ідентифікатори? {#what-are-identifiers}

Ідентифікатор — це частина інформації, яка діє як покажчик на певну особу або особи. До загальних ідентифікаторів відносяться:

- Ім'я
- Номер соціального страхування / податковий номер
- Номер мобільного телефону
- Дата й місце народження
- Цифрові ідентифікаційні дані, як-от адреси електронної пошти, імена користувачів, аватари

Ці традиційні приклади ідентифікаторів видаються, зберігаються й контролюються центральними органами. Вам потрібен дозвіл від уряду вашої країни, щоб змінити своє ім’я, або від платформи соціальних мереж, щоб змінити свій псевдонім.

## Що таке атестації? {#what-are-attestations}

Атестація — це заява, яку зроблено одним суб’єктом відносно іншого суб’єкта. Якщо ви проживаєте в Сполучених Штатах, посвідчення водія, видане вам Департаментом автотранспорту (одним суб’єктом), засвідчує, що ви (інший суб'єкт) маєте право керувати автомобілем на законних підставах.

Атестації відрізняються від ідентифікаторів. Атестація _містить_ ідентифікатори для посилання на певну ідентичність і робить заяву про атрибут, пов'язаний з цією ідентичністю. Отже, ваше посвідчення водія має ідентифікаційні дані (ПІБ, дата народження, адреса), а також є атестацією вашого законного права на керування транспортним засобом.

### Що таке децентралізовані ідентифікатори? {#what-are-decentralized-identifiers}

Традиційні ідентифікатори, як-от ваше юридичне ім’я або адреса електронної пошти, покладаються на третіх осіб — уряди та провайдерів електронної пошти. Децентралізовані ідентифікатори (DID) відрізняються від традиційних — вони не видаються, не управляються і не контролюються жодним центральним органом.

Децентралізовані ідентифікатори видаються, зберігаються й контролюються фізичними особами. Прикладом децентралізованого ідентифікатора є обліковий запис [Ethereum](/developers/docs/accounts/). Ви можете створювати скільки завгодно облікових записів без дозволу будь-кого й без необхідності зберігати їх у центральному реєстрі.

Децентралізовані ідентифікатори зберігаються в розподілених реєстрах (блокчейнах) або однорангових мережах. Це робить DID [глобально унікальними, вирішуваними з високою доступністю та криптографічно перевірюваними](https://w3c-ccg.github.io/did-primer/). Децентралізований ідентифікатор може бути пов’язаний із різними суб'єктами, зокрема людьми, організаціями або державними установами.

## Що уможливлює децентралізовані ідентифікатори? {#what-makes-decentralized-identifiers-possible}

### 1. Інфраструктура відкритих ключів (PKI) {#public-key-cryptography}

Інфраструктура відкритих ключів (ІВК) — це захід інформаційної безпеки, який генерує [відкритий ключ](/glossary/#public-key) і [приватний ключ](/glossary/#private-key) для суб’єкта. Криптографія з відкритим ключем використовується в мережах блокчейн для автентифікації користувачів і підтвердження права власності на цифрові активи.

Деякі децентралізовані ідентифікатори, як-от обліковий запис Ethereum, мають публічні та приватні ключі. Відкритий ключ ідентифікує контролера облікового запису, а закриті ключі дають змогу підписувати й розшифровувати повідомлення для цього облікового запису. PKI надає докази, необхідні для автентифікації суб’єктів і запобігання видавання себе за іншу особу й використання фальшивих ідентифікаційних даних, використовуючи [криптографічні підписи](https://andersbrownworth.com/blockchain/public-private-keys/) для перевірки всіх претензій.

### 2. Децентралізовані сховища даних {#decentralized-datastores}

Блокчейн слугує реєстром даних, який можна перевірити: відкритим, надійним і децентралізованим сховищем інформації. Існування публічних блокчейнів позбавляє необхідності зберігати ідентифікатори в централізованих реєстрах.

Якщо комусь потрібно підтвердити дійсність децентралізованого ідентифікатора, він може знайти відповідний відкритий ключ у блокчейні. Це відрізняється від традиційних ідентифікаторів, які вимагають автентифікації третіх осіб.

## Як децентралізовані ідентифікатори й атестації забезпечують децентралізовану ідентифікацію? {#how-decentralized-identifiers-and-attestations-enable-decentralized-identity}

Децентралізована ідентифікація — це ідея про те, що інформація, пов'язана з ідентифікацією, повинна бути самоконтрольованою, приватною та портативною, а децентралізовані ідентифікатори й атестації є основними будівельними блоками.

У контексті децентралізованої ідентифікації атестації (відомі також як [перевірювані облікові дані](https://www.w3.org/TR/vc-data-model/)) є захищеними від підробки, криптографічно перевіреними твердженнями, зробленими емітентом. Кожна атестація або перевірювані облікові дані, які видаються суб'єктом (наприклад, організацією), пов'язані з їхніми DID.

Оскільки DID зберігаються в блокчейні, будь-хто може перевірити дійсність атестації шляхом перехресної перевірки DID емітента в Ethereum. По суті, блокчейн Ethereum діє як глобальний каталог, який дає змогу перевіряти DID, пов’язані з певними суб'єктами.

Завдяки децентралізованим ідентифікаторам атестації є самоконтрольованими й перевірюваними. Навіть якщо емітента більше не існує, тримач завжди має доказ походження й дійсності атестації.

Децентралізовані ідентифікатори також мають вирішальне значення для захисту конфіденційності особистої інформації шляхом децентралізованої ідентифікації. Наприклад, якщо фізична особа подає підтвердження атестації (водійське посвідчення), стороні, що перевіряє, не потрібно перевіряти правдивість інформації, що міститься у підтвердженні. Натомість верифікатору потрібні лише криптографічні гарантії автентичності атестації та ідентифікація організації, яка його видала, щоб визначити, чи є доказ дійсним.

## Види атестацій у децентралізованій ідентичності {#types-of-attestations-in-decentralized-identity}

Спосіб зберігання й отримання інформації про атестацію в екосистемі ідентифікації на основі Ethereum відрізняється від традиційного управління ідентифікацією. Нижче наведено огляд різних підходів до видачі, зберігання та перевірки посвідчень у децентралізованих системах ідентифікації:

### Атестації поза мережею {#off-chain-attestations}

Однією з проблем, пов’язаних зі зберіганням атестацій у ланцюжку, є те, що вони можуть містити інформацію, яку люди хочуть зберегти конфіденційною. Публічний характер блокчейну Ethereum робить непривабливим зберігання таких атестацій.

Рішення полягає у видачі атестацій, які зберігаються користувачами поза мережею в цифрових гаманцях, але підписані DID емітента, що зберігається в мережі. Ці атестації закодовані як [вебтокени JSON](https://en.wikipedia.org/wiki/JSON_Web_Token) і містять цифровий підпис емітента, що дає змогу легко перевірити заяви поза мережею.

Ось гіпотетичний сценарій для пояснення атестацій поза мережею:

1. Університет (емітент) створює атестацію (цифровий академічний сертифікат), підписує своїми ключами й видає її Бобу (власнику посвідчення).

2. Боб подає заявку на роботу й хоче підтвердити роботодавцю свою академічну кваліфікацію, тому він ділиться атестацією зі свого мобільного гаманця. Потім компанія (верифікатор) може підтвердити дійсність атестації, перевіривши DID емітента (тобто його відкритий ключ в Ethereum).

### Атестації поза мережею з постійним доступом {#offchain-attestations-with-persistent-access}

Відповідно до цієї домовленості атестації перетворюються у файли JSON і зберігаються поза мережею (в ідеалі на платформі [децентралізованого хмарного сховища](/developers/docs/storage/), як-от IPFS або Swarm). Однак [хеш](/glossary/#hash) файлу JSON зберігається в блокчейні й пов’язується з DID через реєстр у блокчейні. Пов’язаний DID може належати або тому, хто видав атестацію, або одержувачу.

Цей підхід дає атестаціям змогу отримати стійкість на основі блокчейну, водночас зберігаючи інформацію про заявку в зашифрованому вигляді й такою, яку можна перевірити. Це також дає змогу вибіркового розкриття, оскільки власник закритого ключа може розшифрувати інформацію.

### Атестації в блокчейні {#onchain-attestations}

Атестації в блокчейні проводяться в [розумних контрактах](/developers/docs/smart-contracts/) у блокчейні Ethereum. Розумний контракт (діючи як реєстр) зіставлятиме атестацію з відповідним децентралізованим ідентифікатором у ланцюжку (відкритим ключем).

Ось приклад, щоб показати, як на практиці можуть працювати атестації в блокчейні:

1. Компанія (XYZ Corp) планує продати частки власності за допомогою розумного контракту, але хоче мати лише покупців, які пройшли перевірку.

2. XYZ Corp може доручити компанії провести перевірку репутації для видачі атестацій у мережі Ethereum. Ця атестація засвідчує, що особа пройшла перевірку репутації без розкриття будь-якої особистої інформації.

3. Розумний контракт на продаж акцій може перевіряти в договорі реєстру особи перевірених покупців, що дає змогу розумному контракту визначати, кому дозволено купувати акції, а кому ні.

### Токени Soulbound та ідентичність {#soulbound}

[Токени Soulbound](https://vitalik.eth.limo/general/2022/01/26/soulbound.html) (NFT, що не підлягають передаванню) можна використовувати для збору інформації, унікальної для певного гаманця. Це фактично створює унікальну ідентифікаційну інформацію в ланцюжку, прив’язану до конкретної адреси Ethereum, яка може містити токени, що представляють досягнення (наприклад, завершення певного онлайн-курсу або проходження порогового значення в грі) або участь у спільноті.

## Переваги децентралізованої ідентичності {#benefits-of-decentralized-identity}

1. Децентралізована ідентифікація підвищує індивідуальний контроль над ідентифікаційною інформацією. Децентралізовані ідентифікатори й атестації можна перевіряти, не покладаючись на централізовані органи та сторонні служби.

2. Децентралізовані рішення для ідентифікації забезпечують безперебійний метод перевірки й управління ідентифікацією користувачів, який не вимагає довіри й захищає конфіденційність.

3. Децентралізована ідентифікація використовує технологію блокчейн, яка створює довіру між різними сторонами й забезпечує криптографічні гарантії для підтвердження дійсності атестацій.

4. Децентралізована ідентичність дає змогу переносити ідентифікаційні дані. Користувачі зберігають атестати й ідентифікатори в мобільному гаманці та можуть обмінюватися ними з будь-якою стороною за власним вибором. Децентралізовані ідентифікатори й атестації не прив'язані до бази даних організації, що їх видала.

5. Децентралізована ідентичність повинна добре працювати з новими технологіями нульового знання, які дадуть людям змогу довести, що вони володіють чимось чи зробили щось, не розкриваючи, що це таке. Це може стати потужним способом поєднання довіри й конфіденційності для різних застосунків, як-от голосування.

6. Децентралізована ідентичність дає механізму протидії атакам Сивілли змогу виявляти випадки, коли одна людина видає себе за іншу, щоб грати або поширювати спам у якійсь системі.

## Випадки використання децентралізованої ідентифікації {#decentralized-identity-use-cases}

Децентралізована ідентифікація має багато потенційних варіантів використання:

### 1. Універсальні логіни {#universal-dapp-logins}

Децентралізована ідентифікація може допомогти замінити парольні входи на [децентралізовану автентифікацію](https://www.ibm.com/blogs/blockchain/2018/10/decentralized-identity-an-alternative-to-password-based-authentication/). Постачальники послуг можуть видавати користувачам атестати, які можуть зберігатися в гаманці Ethereum. Прикладом атестації може бути [NFT](/nft/), що надає власнику доступ до онлайн-спільноти.

Функція [Увійти за допомогою Ethereum](https://login.xyz/) дасть серверам змогу підтвердити обліковий запис користувача Ethereum і отримати необхідне підтвердження з адреси його облікового запису. Це означає, що користувачі можуть отримати доступ до платформ і вебсайтів без необхідності запам'ятовувати довгі паролі й покращує онлайн-досвід для користувачів.

### 2. Автентифікація KYC {#kyc-authentication}

Використання багатьох онлайн-сервісів вимагає від осіб надання атестацій і облікових даних, як-от водійське посвідчення або національний паспорт. Але такий підхід є проблематичним, оскільки приватна інформація користувачів може бути скомпрометована, а постачальники послуг не можуть перевірити справжність атестації.

Децентралізована ідентифікація дає компаніям змогу відмовитися від традиційних процесів [«знай свого клієнта» (KYC)](https://en.wikipedia.org/wiki/Know_your_customer) і автентифікувати ідентифікаційні дані користувачів за допомогою перевірених облікових даних. Це зменшує витрати на управління ідентифікацією та запобігає використанню підроблених документів.

### 3. Голосування й онлайн-спільноти {#voting-and-online-communities}

Онлайн-голосування й соціальні мережі — два нових застосування децентралізованої ідентифікації. Схеми онлайн-голосування піддаються маніпуляціям, особливо якщо зловмисники створюють фальшиві імена для голосування. Прохання до осіб надавати атестації в блокчейні може підвищити чесність процесів онлайн-голосування.

Децентралізована ідентифікація може допомогти створити онлайн-спільноти, вільні від фейкових облікових записів. Наприклад, кожному користувачеві, можливо, доведеться підтверджувати свою особу за допомогою заснованої на блокчейні системи ідентифікації, як-от служба імен Ethereum, що зменшує ймовірність появи ботів.

### 4. Захист від атак Сивілли {#sybil-protection}

Атаки Сивілли — це коли окремі люди обманюють систему, змушуючи її думати, що вони є кількома людьми, щоб збільшити свій вплив. [Програми для надання грантів](https://gitcoin.co/grants/), які використовують [квадратичне голосування](https://www.radicalxchange.org/concepts/plural-voting/), уразливі до цих атак Сивілли, оскільки вартість гранту збільшується, коли за нього голосує більше осіб, що стимулює користувачів розподіляти свої внески між багатьма особами. Децентралізовані ідентифікаційні дані допомагають запобігти цьому, зобов’язуючи на кожного учасника довести, що вони справді люди, хоча часто без необхідності розкривати приватну інформацію.

## Використання децентралізованої ідентифікації {#use-decentralized-identity}

Існує багато амбітних проєктів, що використовують Ethereum як основу для децентралізованої ідентифікації:

- **[Служба імен Ethereum (ENS)](https://ens.domains/)** — _децентралізована система імен для мережевих машинозчитуваних ідентифікаторів, як-от адреси гаманців Ethereum, хеші вмісту й метаданих. _
- **[SpruceID](https://www.spruceid.com/)** — _проєкт децентралізованої ідентифікації, який дає користувачам змогу контролювати цифрову ідентифікацію за допомогою облікових записів Ethereum і профілів ENS замість використання сторонніх служб._
- **[Служба атестації Ethereum (EAS)](https://attest.sh/)** — _децентралізований реєстр/протокол для створення будь-яких атестацій у ланцюжку та поза ним._
- **[Proof of Humanity](https://www.proofofhumanity.id)** — _Доказ людства (або PoH) — це соціальна система підтвердження особистості, побудована на Ethereum._
- **[BrightID](https://www.brightid.org/)** — _децентралізована мережа соціальної ідентифікації з відкритим вихідним кодом, яка прагне реформувати перевірку особистості шляхом створення й аналізу соціального графа._
- **[Паспорт, що підтверджує особу,](https://proofofpersonhood.com/)** — _децентралізований агрегатор цифрових ідентифікаційних даних._

## Довідкові джерела {#further-reading}

### Статті {#articles}

- [Випадки використання блокчейну: блокчейн у цифровій ідентифікації](https://consensys.net/blockchain-use-cases/digital-identity/)—_ConsenSys_
- [Що таке Ethereum ERC725? Самостійне керування ідентифікацією в блокчейні](https://cryptoslate.com/what-is-erc725-self-sovereign-identity-management-on-the-blockchain/) — _Sam Town_
- [Як блокчейн може розв’язувати проблему цифрової ідентичності](https://time.com/6142810/proof-of-humanity/) — _Ендрю Р. Чоу_
- [Що таке децентралізована ідентифікація і чому це має вас хвилювати?](https://web3.hashnode.com/what-is-decentralized-identity) — _Еммануель Авосіка_

### Відео {#videos}

- [Децентралізована ідентифікація (бонусна сесія в прямому ефірі)](https://www.youtube.com/watch?v=ySHNB1za_SE&t=539s) — _Чудове пояснювальне відео про децентралізовану ідентифікацію від Андреаса Антонополуса_
- [Увійдіть за допомогою Ethereum і децентралізованої ідентифікації за допомогою Ceramic, IDX, React і 3ID Connect](https://www.youtube.com/watch?v=t9gWZYJxk7c) — _Посібник на YouTube зі створення системи керування ідентифікацією для створення, читання й оновлення профілю користувача профіль за допомогою його гаманця Ethereum від Надер Дебіт_
- [BrightID – децентралізована ідентифікація в Ethereum](https://www.youtube.com/watch?v=D3DbMFYGRoM) — _подкаст безкоштовних версій, у якому обговорюється BrightID, децентралізоване рішення ідентифікації для Ethereum_
- [Інтернет поза ланцюгом: децентралізована ідентифікація та перевірювані повноваження](https://www.youtube.com/watch?v=EZ_Bb6j87mg) — презентація EthDenver 2022 від Евіна Мак-Маллена

### Спільноти {#communities}

- [Альянс ERC-725 на GitHub](https://github.com/erc725alliance) — _Прихильники стандарту ERC725 для керування ідентифікацією в блокчейні Ethereum_
- [Сервер Discord SpruceID](https://discord.com/invite/Sf9tSFzrnt) — _Спільнота для ентузіастів і розробників, які працюють над входом за допомогою Ethereum_
- [Veramo Labs](https://discord.gg/sYBUXpACh4) — _спільнота розробників, які роблять внесок у створення основи для перевірених даних для програм_