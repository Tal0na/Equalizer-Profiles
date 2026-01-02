# Профили эквалайзера

[![en](https://img.shields.io/badge/lang-en-red.svg)](/README/README.md)
[![pt-BR](https://img.shields.io/badge/lang-pt--BR-green.svg)](/README/README.pt-BR.md)
[![ru](https://img.shields.io/badge/lang-ru-yellow.svg)](/README/README.ru.md)
[![uk-UA](https://img.shields.io/badge/lang-uk--UA-blue.svg)](/README/README.uk-UA.md)

## Введение

Этот репозиторий содержит **пользовательские профили эквалайзера**, предназначенные для улучшения качества звука в системах **Windows и Linux**.  
Профили подходят для музыки, игр, фильмов и общего мультимедийного использования и могут быть адаптированы под разные аудиоустройства и личные предпочтения.

---

## Поддерживаемые платформы и приложения

### Windows
- **Equalizer APO**
- **Peace Equalizer** (графический интерфейс для Equalizer APO)

### Linux
- **EasyEffects** (PipeWire — рекомендуется)
- **PulseEffects** (PulseAudio — устаревшее решение)
- **Встроенные эквалайзер-фильтры PipeWire**

> ⚠️ Большинство современных дистрибутивов Linux (Fedora, Arch, Ubuntu 22.10+) по умолчанию используют **PipeWire**.  
> В этом случае рекомендуется использовать **EasyEffects**.

---

## Требования

### Windows
- **Equalizer APO**  
  https://sourceforge.net/projects/equalizerapo/
- **Peace Equalizer**  
  https://sourceforge.net/projects/peace-equalizer-apo-extension/

### Linux
- **EasyEffects**
  - Flatpak (рекомендуется):
    ```bash
    flatpak install flathub com.github.wwmm.easyeffects
    ```
  - Или установка через менеджер пакетов вашего дистрибутива
- **PipeWire** (обычно установлен по умолчанию)

---

## Категории

Профили эквалайзера организованы по **типу аудиоустройства**:

- **Earphones**  
  Внутриканальные наушники, такие как IEM и earbuds (проводные или беспроводные).

- **Headphones**  
  Полноразмерные и накладные наушники для прослушивания музыки, мониторинга и общего использования.

- **Headsets (Gamer)**  
  Игровые гарнитуры со встроенным микрофоном, оптимизированные для игр, голосового чата и мультимедиа.

- **Speakers**  
  Настольные колонки, полочные акустические системы и традиционные динамики.

- **Soundbars**  
  Саундбары, используемые с телевизорами, мониторами или настольными системами.

Эта структура обеспечивает единообразие между  
**Windows (Peace / Equalizer APO)** и **Linux (EasyEffects / PipeWire / PulseEffects)**.

---

## Как применить профили

### Windows (Peace Equalizer)

1. Откройте **Peace Equalizer**.
2. Настройте частотные полосы и фильтры в соответствии с профилем.
3. Нажмите **Save settings** и задайте имя профиля  
   Пример: `MyEQConfig`.
4. Для загрузки профиля:
   - Откройте Peace Equalizer
   - Перейдите в **Presets**
   - Выберите `MyEQConfig`

---

### Linux (EasyEffects)

1. Откройте **EasyEffects**.
2. Включите эффект **Equalizer**.
3. Настройте частотные полосы вручную или импортируйте пресет.
4. Нажмите **Presets → Save Preset**.
5. (Необязательно) Назначьте пресет для:
   - Системного вывода
   - Отдельных приложений

> EasyEffects поддерживает **профили для отдельных приложений**, чего нет в Equalizer APO.

---

## Примечания о совместимости профилей

- Частотные полосы и значения усиления **полностью совместимы** между:
  - Peace Equalizer ↔ EasyEffects
- Названия некоторых фильтров могут отличаться:
  - **Preamp** → **Input Gain**
  - **Peak Filter** → **Bell Filter**
- Всегда настраивайте **preamp/input gain**, чтобы избежать клиппинга и искажений.

---

## Заключительные замечания

Эти профили основаны на **личных предпочтениях** и могут не подойти:
- Для всех гарнитур, наушников или колонок
- Для всех музыкальных жанров и сценариев использования

Вы можете свободно изменять:
- Уровни усиления
- Значения Q
- Громкость предусилителя

Если вы улучшили или адаптировали профиль под конкретное устройство, поделитесь им с сообществом.

---

## Ссылки

- Документация Equalizer APO  
  https://sourceforge.net/p/equalizerapo/wiki/Documentation/
- Руководство пользователя Peace Equalizer  
  https://sourceforge.net/p/peace-equalizer-apo-extension/wiki/Documentation/
- Документация EasyEffects  
  https://github.com/wwmm/easyeffects
