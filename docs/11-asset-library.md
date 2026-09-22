# 11. Asset library

Status: `v1.0 / production`

## Brand assets

`assets/brand/` содержит четыре и только четыре официальных production PNG:

- `cu-logo-full-black.png` — full logo для светлого фона;
- `cu-logo-full-white.png` — full logo для тёмного фона;
- `cu-mark-black.png` — compact mark для светлого фона;
- `cu-mark-white.png` — compact mark для тёмного фона.

Full logo нужен для полной идентификации. Compact mark — разрешённая левая геометрическая часть для формы, малых digital placements, аватаров, паттернов, углов карточек и внутренних слайдов. Нельзя создавать производные цветные версии, менять геометрию или генерировать logo через GPT Image.

## Generated assets

`assets/generated/<family>/<object>/<object>_<mode>_vNN.png`.

Families: `orienteering`, `tourism`, `climbing`, `environment`, `campaign`. Status: `draft` вне production, `candidate`, `master`, `deprecated`. Каждый candidate/master связан с versioned prompt.

## Custom Emoji

`assets/custom-emoji/` — production-набор клубных Custom Emoji для постов, анонсов и реакций.

- `masters/` — исходники высокого разрешения для правок и новых экспортов;
- `telegram-100x100/` — статичные PNG 100×100 px с прозрачностью, готовые к загрузке в Telegram;
- `preview.png` — визуальная проверка полного набора на тёмном фоне;
- `README.md` — семантика, Unicode-привязки и инструкция по публикации.

Новый символ добавляется только вместе с master-файлом, Telegram-экспортом и строкой в таблице Unicode-привязок. Визуальный язык набора: объёмный premium 3D/embossed pictogram, deep dark navy, толстый белый keyline, vivid signal orange `#FC8A05`, мягкие controlled highlights, Route Line и ясный силуэт без текста. Плоская outline-стилизация не используется.

## Naming and provenance

Имена — lowercase kebab-case, версия `vNN`. В описании/sidecar фиксируются prompt, дата, crop, intended use, status и известные ограничения. Запрещены чужие коммерческие logo, AI-gibberish и непроверенные license sources.
