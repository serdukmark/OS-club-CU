# 14. Governance

Status: `v1.0 / production`

`main` — единственный утверждённый source of truth. Версия следует Semantic Versioning: patch — уточнение без изменения поведения; minor — новый совместимый template/asset family; major — изменение core identity или обязательных правил.

## Protected decisions

Review обязателен для logo assets, core palette, canonical formats, spacing base, typography source и правила Route Line. Четыре PNG в `assets/brand/` нельзя заменять производными или generated версиями.

## Logo governance

Разрешены Full CU logo и Compact CU mark в black/white. Compact mark официально допустим для apparel, small digital, avatars, patterns, card corners и internal slides. Любое новое исполнение должно быть получено из официального source и отдельно утверждено; автоматическая трассировка и GPT Image не являются источником.

## Change process

Каждое системное изменение содержит rationale, затронутые носители, обновлённую документацию/templates/tokens и запись в `CHANGELOG.md`. Deprecated asset не удаляется без миграционного периода, если на него ссылаются активные материалы.

## Ownership

Владелец бренда подтверждает visual rules; владелец события — факты; дизайнер — layout/preflight; производитель — технические допуски. Один человек может выполнять несколько ролей, но проверки остаются раздельными.
