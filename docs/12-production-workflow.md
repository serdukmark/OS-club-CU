# 12. Production workflow

Status: `v1.0 / mandatory`

## Flow

1. Brief: цель, аудитория, формат, канал, дедлайн и владелец фактов.
2. Content: утвердить title, date/time, place, CTA, URL и legal/sponsor data.
3. Format: выбрать canonical canvas из `design/format-specs.json`.
4. Visual: фотография или GPT Image asset; для генерации использовать versioned prompt.
5. Layout: применить токены, grid, Route Line и официальный logo PNG отдельными слоями.
6. Review: content, brand, accessibility, technical export.
7. Export: master + delivery file; проверить реальные размеры.
8. Archive: сохранить editable source, финальный export, prompt и approval note.

## Preflight

- один главный message и ясная иерархия;
- факты сверены человеком-владельцем;
- logo взят из `assets/brand/`, не искажён и имеет правильную контрастную версию;
- QR создан в layout, протестирован с экрана/печати;
- generated image не содержит финальных дат, текста или псевдологотипа;
- safe margins, contrast, captions/alt text и export profile проверены;
- нет draft assets, временных архивов и мусорных файлов.

Production считается завершённым только после просмотра финального экспортированного файла, а не только editable layout.
