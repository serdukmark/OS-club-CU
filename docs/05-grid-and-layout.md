# 05. Grid and layout

Status: `v1.0 / production`

## Canonical canvases

- Social feed: 1080×1350, safe margin 72 px.
- Square: 1080×1080, safe margin 64 px.
- Story / digital poster: 1080×1920, safe margin 72 px; учитывать UI-зоны сверху и снизу.
- Presentation: 1920×1080, safe margin 96 px.

Точные значения находятся в `design/format-specs.json`.

## Grid

Основная сетка — 12 колонок для feed/presentation и 6 колонок для story. Gutter кратен 8 px. Заголовок, data block и visual anchor должны иметь ясные зоны; визуал не используется как фон для длинного текста без контрастной поверхности.

## Route Line

Линия маршрута связывает смысловые точки: дату с местом, этапы с результатами, карточки карусели. Она не пересекает логотип, основной заголовок, лица и QR. В карусели допускается визуальное продолжение линии между слайдами, но каждый слайд должен работать отдельно.

## Logo placement

Full logo выбирается, когда ширина позволяет прочитать wordmark. Compact mark — в малых углах, внутренних слайдах, avatar/pattern и apparel. Логотип масштабируется равномерно и сохраняет прозрачное поле; white — на dark, black — на light.
