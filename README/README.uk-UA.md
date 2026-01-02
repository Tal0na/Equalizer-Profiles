# Профілі еквалайзера

[![en](https://img.shields.io/badge/lang-en-red.svg)](/README/README.md)
[![pt-BR](https://img.shields.io/badge/lang-pt--BR-green.svg)](/README/README.pt-BR.md)
[![ru](https://img.shields.io/badge/lang-ru-yellow.svg)](/README/README.ru.md)
[![uk-UA](https://img.shields.io/badge/lang-uk--UA-blue.svg)](/README/README.uk-UA.md)

## Вступ

Цей репозиторій містить **користувацькі профілі еквалайзера**, створені для покращення якості звуку в системах **Windows та Linux**.  
Профілі призначені для музики, ігор, фільмів і загального мультимедійного використання та можуть бути адаптовані під різні аудіопристрої й особисті вподобання.

---

## Підтримувані платформи та застосунки

### Windows
- **Equalizer APO**
- **Peace Equalizer** (графічний інтерфейс для Equalizer APO)

### Linux
- **EasyEffects** (PipeWire — рекомендовано)
- **PulseEffects** (PulseAudio — застаріле)
- **Вбудовані фільтри еквалайзера PipeWire**

> ⚠️ Більшість сучасних дистрибутивів Linux (Fedora, Arch, Ubuntu 22.10+) за замовчуванням використовують **PipeWire**.  
> У цьому випадку рекомендується **EasyEffects**.

---

## Вимоги

### Windows
- **Equalizer APO**  
  https://sourceforge.net/projects/equalizerapo/
- **Peace Equalizer**  
  https://sourceforge.net/projects/peace-equalizer-apo-extension/

### Linux
- **EasyEffects**
  - Flatpak (рекомендовано):
    ```bash
    flatpak install flathub com.github.wwmm.easyeffects
    ```
  - Або встановлення через менеджер пакетів вашого дистрибутива
- **PipeWire** (зазвичай встановлений за замовчуванням)

---

## Категорії

Профілі еквалайзера впорядковані за **типом аудіопристрою**:

- **Earphones**  
  Внутрішньоканальні пристрої, такі як IEM та earbuds (дротові або бездротові).

- **Headphones**  
  Повнорозмірні та накладні навушники для прослуховування музики, моніторингу та загального використання.

- **Headsets (Gamer)**  
  Ігрові гарнітури з вбудованим мікрофоном, оптимізовані для ігор, голосового чату та мультимедіа.

- **Speakers**  
  Настільні колонки, поличкові акустичні системи та традиційні динаміки.

- **Soundbars**  
  Саундбари для використання з телевізорами, моніторами або настільними сетапами.

Ця структура забезпечує узгодженість між  
**Windows (Peace / Equalizer APO)** та **Linux (EasyEffects / PipeWire / PulseEffects)**.

---

## Як застосувати профілі

### Windows (Peace Equalizer)

1. Відкрийте **Peace Equalizer**.
2. Налаштуйте смуги частот і фільтри відповідно до профілю.
3. Натисніть **Save settings** і задайте назву профілю  
   Приклад: `MyEQConfig`.
4. Щоб завантажити профіль:
   - Відкрийте Peace Equalizer
   - Перейдіть до **Presets**
   - Оберіть `MyEQConfig`

---

### Linux (EasyEffects)

1. Відкрийте **EasyEffects**.
2. Увімкніть ефект **Equalizer**.
3. Налаштуйте смуги частот вручну або імпортуйте пресет.
4. Натисніть **Presets → Save Preset**.
5. (Необов’язково) Призначте пресет для:
   - Системного виводу
   - Окремих застосунків

> EasyEffects підтримує **профілі для окремих застосунків**, чого немає в Equalizer APO.

---

## Нотатки щодо сумісності профілів

- Смуги частот і значення підсилення **повністю сумісні** між:
  - Peace Equalizer ↔ EasyEffects
- Назви деяких фільтрів можуть відрізнятися:
  - **Preamp** → **Input Gain**
  - **Peak Filter** → **Bell Filter**
- Завжди налаштовуйте **preamp/input gain**, щоб уникнути кліпінгу та спотворень.

---

## Заключні зауваження

Ці профілі базуються на **особистих уподобаннях** і можуть не підходити:
- Для всіх гарнітур, навушників або колонок
- Для всіх музичних жанрів чи сценаріїв використання

Ви можете вільно змінювати:
- Рівні підсилення
- Значення Q
- Гучність preamp

Якщо ви покращили або адаптували профіль під конкретний пристрій, поділіться ним зі спільнотою.

---

## Посилання

- Документація Equalizer APO  
  https://sourceforge.net/p/equalizerapo/wiki/Documentation/
- Посібник користувача Peace Equalizer  
  https://sourceforge.net/p/peace-equalizer-apo-extension/wiki/Documentation/
- Документація EasyEffects  
  https://github.com/wwmm/easyeffects
