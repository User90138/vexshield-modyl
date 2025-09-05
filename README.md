[README.md](https://github.com/user-attachments/files/22181687/README.md)

# VexShield (VSH) — статический сайт

Готовый к деплою архив для GitHub Pages или Vercel.

## Структура
- `index.html` — главная (виджет цены, живая строка, ключевые функции)
- `pages/tokenomics.html` — токеномика, модули AntiDump
- `pages/nft.html` — NFT ShieldPass (права, интеграции, SDK)
- `pages/airdrop.html` — визуальный airdrop (email + условие ≥5 USDT Base)
- `pages/checkin.html` — Daily Check‑in (серия до 7 дней, без обнуления)
- `pages/bonding.html` — Bonding (пока неактивен)
- `pages/admin.html` — Админ‑панель (демо)
- `pages/faq.html`, `pages/contact.html`
- `assets/css/style.css`, `assets/js/utils.js`, `assets/img/logo.svg`

## Деплой на GitHub Pages
1. Создайте репозиторий `vexshield.github.io` (или `User90138.github.io/vexshield` для проекта).
2. Загрузите содержимое архива в корень репозитория.
3. В Settings → Pages выберите ветку `main` / `/ (root)`. Через 1–2 минуты сайт будет доступен.

## Деплой на Vercel
1. Импортируйте репозиторий.
2. Проект — «Other». Build Command: none, Output: `/`.
3. Deploy.

## Настройка
- Реальные данные цен можно подключить в `assets/js/utils.js` внутри `loadPriceWidget`.
- Ончейн‑проверки email и USDT Base заменены заглушками (см. `Airdrop` страница).
- Ограничение «1 IP раз в 7 дней» воспроизведено локально через `localStorage` (демо).

## Примечание
Всё работает без бэкенда (статично). Для продакшена подключите API/сервер.
