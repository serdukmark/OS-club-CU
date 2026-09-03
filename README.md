# Brand OS клуба ЦУ

Версия: `1.0`

Операционная система бренда клуба «Спортивное ориентирование и туризм» Центрального университета для постов, каруселей, Stories, презентаций, плакатов, фотоотчётов, формы и мерча.

## Формула бренда

**Central University × Outdoor × Orienteering × Tourism**

Визуальная дисциплина ЦУ соединяется с движением, маршрутом, картой, высотой, командой и техническим снаряжением. Результат должен выглядеть как современный университетский outdoor-tech бренд, а не как generic green tourism aesthetic.

База системы: near-black, white и cold/light gray. Главный клубный акцент — signal orange `#FC8A05`. Главный графический мотив — **Route Line**.

## Официальная система логотипа

В репозитории разрешены ровно четыре production-asset:

| Вариант | Файл | Применение |
| --- | --- | --- |
| Full Black | [`assets/brand/cu-logo-full-black.png`](assets/brand/cu-logo-full-black.png) | Полная идентификация на светлом фоне |
| Full White | [`assets/brand/cu-logo-full-white.png`](assets/brand/cu-logo-full-white.png) | Полная идентификация на тёмном фоне |
| Compact Mark Black | [`assets/brand/cu-mark-black.png`](assets/brand/cu-mark-black.png) | Компактное размещение на светлом фоне |
| Compact Mark White | [`assets/brand/cu-mark-white.png`](assets/brand/cu-mark-white.png) | Компактное размещение на тёмном фоне |

Compact mark — только левая геометрическая часть официального логотипа. Это разрешённая версия для формы, кепок, баффов, рюкзаков, аватаров, паттернов, углов карточек, внутренних слайдов и небольших digital placements.

Логотип нельзя перерисовывать, растягивать, перекрашивать в orange/violet, снабжать эффектами или генерировать через GPT Image. GPT Image создаёт только визуальные изображения и hero assets; официальный PNG накладывается отдельным production-слоем.

## Быстрый старт

1. Выберите носитель и формат из [`design/format-specs.json`](design/format-specs.json).
2. Возьмите подходящий brief из [`templates/`](templates/).
3. Используйте токены из [`design/tokens.json`](design/tokens.json).
4. При необходимости создайте visual по versioned prompt из [`prompts/master/`](prompts/master/).
5. Соберите редактируемый layout: типографика, фактические данные, QR, Route Line и официальный logo asset.
6. Проведите preflight по [`docs/12-production-workflow.md`](docs/12-production-workflow.md) и экспорт по [`docs/16-accessibility-export.md`](docs/16-accessibility-export.md).

## Структура

- [`assets/brand/`](assets/brand/) — официальные PNG логотипа ЦУ;
- [`assets/generated/`](assets/generated/) — утверждённые GPT Image visuals;
- [`design/`](design/) — machine-readable токены и форматы;
- [`docs/`](docs/) — спецификации Brand OS;
- [`templates/`](templates/) — production briefs;
- [`prompts/master/`](prompts/master/) — versioned prompts для визуалов.

## Основные документы

- [Brand foundation](docs/01-brand-foundation.md)
- [Content system](docs/02-content-system.md)
- [GPT Image pipeline](docs/03-gpt-image-pipeline.md)
- [Design tokens](docs/04-design-tokens.md)
- [Grid and layout](docs/05-grid-and-layout.md)
- [Social posts](docs/06-social-posts.md)
- [Presentations](docs/07-presentations.md)
- [Posters](docs/08-posters.md)
- [Apparel](docs/09-apparel.md)
- [Photography and video](docs/10-photography-and-video.md)
- [Asset library](docs/11-asset-library.md)
- [Production workflow](docs/12-production-workflow.md)
- [Do / Don’t](docs/13-do-dont.md)
- [Governance](docs/14-governance.md)
- [Copy system](docs/15-copy-system.md)
- [Accessibility and export](docs/16-accessibility-export.md)

## Source of truth

`main` содержит актуальную утверждённую версию. Изменения в логотипе, core tokens и обязательных production rules принимаются только через review и фиксируются в [`CHANGELOG.md`](CHANGELOG.md).
