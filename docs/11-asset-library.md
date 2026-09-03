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

## Naming and provenance

Имена — lowercase kebab-case, версия `vNN`. В описании/sidecar фиксируются prompt, дата, crop, intended use, status и известные ограничения. Запрещены чужие коммерческие logo, AI-gibberish и непроверенные license sources.
