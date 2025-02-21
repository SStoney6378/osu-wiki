---
tags:
  - red line
  - red offset
  - red timing point
  - uninherited offset
  - green line
  - green offset
  - green timing point
  - inherited offset
  - timing setup
  - copy timing
  - paste timing
  - красная полоска
  - красные полоски
  - красный оффсет
  - зеленая полоска
  - зеленые полоски
  - зеленый оффсет
  - настройка тайминга
  - копировать тайминг
  - вставить тайминг
---

# Вкладка Timing

*О настройке тайминга карты см. [Настройка тайминга](/wiki/Guides/How_to_time_songs)*\
*См. также: [Тайминг](/wiki/Beatmapping/Timing)*

**Timing** — вкладка в [редакторе карт](/wiki/Client/Beatmap_editor), на которой можно настроить тайминг [карты](/wiki/Beatmap) для того, чтобы правильно замапать песню. На этой вкладке расположены настройки и инструменты, связанные с таймингом, а также [отдельное окно](#окно-настройки-тайминга) для работы с несколькими [тайминг-секциями](#тайминг-секции) сразу — как для описания музыкальной структуры песни, так и для оформления карты.

## Тайминг-секции

*См. также: [Оффсет](/wiki/Offset)*

*Тайминг-секция* (иногда — *оффсет*) — инструмент [маппинга](/wiki/Beatmapping), позволяющий поменять на определённом отрезке карты сразу несколько общих параметров: [тайминг](/wiki/Beatmapping/Timing), [скорость слайдеров](/wiki/Gameplay/Hit_object/Slider/Slider_velocity), [хитсаунды](/wiki/Beatmapping/Hitsound) или их громкость. В osu! существует два типа тайминг-секций: те, что меняют настройки тайминга («красные»), и те, что его не трогают («зелёные»).

### Красные тайминг-секции

::: Infobox
![](img/uninherited-points.png "Несколько красных тайминг-секций в окне настройки тайминга")
:::

**«Красные»** секции (англ. *uninherited timing point*) имеют свои собственные настройки тайминга и применяются для того, чтобы передать изменения в структуре песни — например, её [скорость](/wiki/Music_theory/Tempo), неравномерно расположенные ноты или меняющийся [размер такта](/wiki/Music_theory/Time_signature). Добавление новой красной секции сбрасывает метроном, после чего он начинает отсчитывать ноты с момента начала секции, называемого оффсетом и измеряемого в миллисекундах.

Помимо корректировки тайминга, с помощью красных секций можно скрывать полосы, обозначающие начало нового такта на игровом поле в [osu!taiko](/wiki/Game_mode/osu!taiko) и [osu!mania](/wiki/Game_mode/osu!mania).

Красные тайминг-секции получили своё жаргонное название из-за того, что они обозначаются красным цветом как в [окне настройки тайминга](#окно-настройки-тайминга), так и на обеих временны́х шкалах.

### Зелёные тайминг-секции

::: Infobox
![](img/inherited-points.png "Несколько зелёных тайминг-секций, имеющих различные настройки киаи, громкости звука и скорости слайдеров")
:::

**«Зелёные»** секции (англ. *inherited timing point*), в отличие от красных, используют уже имеющиеся настройки тайминга. Они применяются для следующих целей:

- Изменение [скорости слайдеров](/wiki/Gameplay/Hit_object/Slider/Slider_velocity)
- Настройка уровня громкости [хитсаундов](/wiki/Beatmapping/Hitsound)
- Переключение между [наборами хитсаундов](/wiki/Beatmapping/Sampleset)
- Включение или выключение [киаи](/wiki/Gameplay/Kiai_time)

Зелёные тайминг-секции получили своё жаргонное название из-за того, что они обозначаются зелёным цветом как в [окне настройки тайминга](#окно-настройки-тайминга), так и на обеих временны́х шкалах.

## Основной вид

![Скриншот вкладки Timing в редакторе](/wiki/shared/timing/Timing_base.jpg)

Вкладку Timing можно открыть с помощью клавиши `F3`. Она позволяет менять следующие настройки:

| Название | Значение |
| :-- | :-- |
| `BPM` | [Скорость](/wiki/Music_theory/Tempo) музыки в текущей тайминг-секции, которая измеряется в ударах в минуту (BPM). |
| `Offset` | [Оффсет](/wiki/Offset#маппинг) текущей тайминг-секции в миллисекундах. |
| `Move already placed notes when changing the offset/BPM` | В ходе настройки тайминга все объекты будут оставаться на своих тиках [временно́й шкалы](/wiki/Client/Beatmap_editor/Timelines). |
| `Slider Velocity` | Базовая [скорость слайдеров](/wiki/Gameplay/Hit_object/Slider/Slider_velocity) на всей карте. |
| `Slider Tick Rate` | Число [слайдер-тиков](/wiki/Gameplay/Hit_object/Slider/Slider_tick) в одной музыкальной [доле](/wiki/Music_theory/Beat). |

Для более точной или грубой настройки можно использовать клавиши-модификаторы, влиюящие на скорость изменения настроек:

|  | Скорость музыки | Оффсет | Скорость слайдеров |
| :-- | :--: | :--: | :--: |
| `Ctrl` + нажатие | 0.25 BPM | 1 мс | 1 [osu!-пиксель](/wiki/Client/Beatmap_editor/osu!_pixel) |
| Обычное нажатие | 1 BPM | 2 мс | 10 osu!-пикселей |
| `Shift` + нажатие | 5 BPM | 10 мс | - |

### Метроном

![](img/metronome.png "Метроном osu! на вкладке тайминга")

Метроном — расположенный в правом верхнем углу экрана индикатор, который помогает быстро подобрать приблизительные настройки тайминга для песни. Чтобы определить примерную скорость песни и оффсет аудио, необходимо в такт музыке нажимать клавишу `T`, либо кликать по кнопке с надписью `Tap Here!`.

Визуально метроном спроектирован под 4/4 — самый популярный [размер музыкального такта](/wiki/Music_theory/Time_signature). Первая секция метронома, мигающая зелёным, обозначает [сильную долю](/wiki/Music_theory/Downbeat), а остальные, пульсирующие белым в такт песне, — слабые доли [такта](/wiki/Music_theory/Measure). Нестандартные размеры такта, например, 7/4, приводят к увеличению числа вспышек на метрономе, но его внешний вид не меняется.

## Окно настройки тайминга

![Скриншот окна настройки тайминга](/wiki/shared/timing/TimingSetup.png)

Окно настройки тайминга можно открыть с помощью клавиши `F6`. Оно позволяет добавлять новые тайминг-секции и изменять настройки уже существующих из них: тайминг песни, [хитсаунды](/wiki/Beatmapping/Hitsound), громкость звука, [наборы хитсаундов](/wiki/Beatmapping/Sampleset) и спецэффекты.

### Выделение и копирование

Все действия в окне настройки тайминга влияют только на выделенные тайминг-секции.

- Чтобы выбрать несколько разных секций, кликните по ним, удерживая `Ctrl`.
- Чтобы выбрать несколько секций подряд, кликните по первой из них, затем зажмите `Shift` и кликните по последней.
- **Чтобы скопировать секции из окна тайминга или вставить их туда**, пользуйтесь стандартными горячими клавишами операционной системы — наиример, `Ctrl` + `C` и `Ctrl` + `V`.
