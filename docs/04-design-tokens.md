# 04. Design tokens

Status: `v1.0 / production`

Machine-readable source: `design/tokens.json`.

## Color

- Signal Orange `#FC8A05` — главный клубный акцент, CTA, Route Line и контрольные точки.
- Dark `#0D0D0F`, `#151518`, `#232329` — основные тёмные поверхности.
- Light `#D8D8DC`, `#F2F2F4`, `#FFFFFF` — холодные светлые поверхности и текст на dark.

На одном носителе обычно один яркий акцент. Orange не используется как цвет логотипа ЦУ. Generic green palette не является частью core identity.

## Spacing and shape

Базовый шаг — `8 px`. Рабочая шкала: 8, 16, 24, 32, 48, 64, 96, 128. Радиусы: 16, 24 и 40 px; pill применяется только для коротких tags/chips. Route Line: 4 px в digital и 8 px на крупных форматах, с оптической коррекцией.

## Typography

Используется подтверждённое официальное семейство ЦУ. Пока его название не внесено из авторитетного source, нельзя объявлять системный fallback официальным. Иерархия: Hero, Section, Operational Data, Body, Micro.

## Token governance

HEX, format sizes, logo paths и spacing меняются сначала в JSON, затем в документации и шаблонах. Произвольные локальные значения не становятся новыми токенами без review.
