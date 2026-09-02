# 03. GPT Image production pipeline

Status: `v0.1 / mandatory`

Цель pipeline — получать не разрозненные картинки, а библиотеку визуалов, которые ощущаются как один бренд и могут многократно использоваться в карточках, презентациях и плакатах.

## 1. Mandatory rule

Все ключевые предметные визуалы и hero illustrations создаются GPT Image.

Запрещено использовать в финальном production как замену:

- схематичные самодельные пиктограммы;
- случайные stock icons;
- дешёвые 3D assets из несогласованных библиотек;
- визуалы, сгенерированные в принципиально разных стилях;
- временные заглушки, которые затем случайно остаются в публикации.

## 2. Asset hierarchy

### Tier 1 — Master hero assets

Самые сильные объекты бренда. Генерируются и отбираются особенно тщательно.

Первая очередь:

1. orienteering control prism;
2. technical carabiner;
3. compass;
4. climbing rope;
5. expedition backpack;
6. headlamp;
7. ice axe;
8. trekking boot.

### Tier 2 — Supporting objects

- helmet;
- electronic punching chip;
- tent;
- stove;
- thermos;
- harness;
- ascender;
- crampons;
- trekking poles;
- checkpoint stand.

### Tier 3 — Environmental / atmospheric assets

- topographic terrain fragments;
- wet night forest surfaces;
- snow / rock / fog environments;
- map-like terrain compositions;
- abstract route environments.

## 3. Master art direction

Все master objects должны принадлежать одному миру.

### Visual target

Premium outdoor technical campaign + contemporary product CGI + CU cleanliness.

### Object properties

- real-world believable geometry;
- premium material detail;
- controlled studio or cinematic light;
- matte technical polymer, textile, brushed/anodized metal;
- club orange as purposeful signal accent;
- white / graphite / metallic support palette;
- no logos from commercial outdoor brands;
- no accidental text, pseudo-labels or gibberish;
- no cartoon proportions;
- no generic app-icon rendering.

## 4. Generation variants

Для каждого master object требуется минимум четыре композиционных режима.

### Hero 01 — clean studio

Изолированный предмет, пригодный для светлых модульных карточек.

### Hero 02 — dark campaign

Тёмный фон, драматичный свет, пригодный для poster / night mode.

### Hero 03 — macro detail

Очень крупный фрагмент материала / механизма для фонового использования.

### Hero 04 — dynamic

Предмет встроен в физическое действие: натянутая верёвка, мокрый компас, призма в лесу и т. п., но без человека, если человек не является смыслом конкретного материала.

## 5. Consistency checks

Перед утверждением визуала проверить:

- совпадает ли orange с системой;
- выглядит ли материал физически убедительно;
- нет ли лишних цветов;
- нет ли случайных надписей;
- не похож ли объект на product ad чужого бренда;
- есть ли свободная зона для верстки;
- работает ли изображение в crop `4:5`, `1:1`, `9:16`, `16:9`;
- сохраняется ли качество при крупном плакатном использовании;
- сочетается ли оно с уже утверждёнными master assets.

## 6. Prompt versioning

Каждый утверждённый asset получает:

- slug;
- version;
- category;
- generation brief;
- intended crops;
- approval status;
- notes about light / material / camera;
- link/path to final image.

Пример структуры:

```text
prompts/
  master/
    control-prism-v01.md
    carabiner-v01.md
    compass-v01.md
```

## 7. File naming

```text
assets/gpt-image/<family>/<object>/<object>_<mode>_vNN.<ext>
```

Пример:

```text
assets/gpt-image/orienteering/control-prism/control-prism_clean-studio_v01.png
assets/gpt-image/climbing/carabiner/carabiner_dark-campaign_v01.png
```

## 8. Approval statuses

- `draft` — генерация на просмотр;
- `candidate` — визуально подходит, проверяем в макетах;
- `master` — утверждён как часть бренд-системы;
- `deprecated` — больше не использовать.

## 9. No-layout generation rule

По умолчанию GPT Image создаёт **сам визуальный asset**, а не весь финальный пост с мелким текстом.

Причина: типографика, даты, адреса, QR и системные метки должны оставаться воспроизводимыми и редактируемыми в layout layer.

Исключение: экспериментальный арт-постер, где типографика сама является частью изображения и затем проходит ручную проверку.

## 10. First production batch

Первая итерация должна доказать стиль всего бренда на пяти объектах:

1. control prism;
2. carabiner;
3. compass;
4. rope;
5. expedition backpack.

После утверждения этих пяти объектов запрещено расширять библиотеку до тех пор, пока они не протестированы минимум на:

- одном анонсе;
- одном фотоотчёте;
- одном expedition poster;
- одном презентационном слайде.
