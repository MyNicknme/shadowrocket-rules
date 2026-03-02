# 🚀 Shadowrocket Config & Auto-Updating Rules

Набор оптимизированных правил для Shadowrocket, разделенных по сервисам. Идеально подходит для всех городов.

---

## 📥 Варианты установки

### 1. Режим "Stable" (Рекомендуемый)
**Логика:** Умная маршрутизация. Банки, Госуслуги, Apple и китайские сервисы (Poizon/Alipay) идут **напрямую**. Все заблокированные ресурсы и остальной зарубежный трафик — **через прокси**.
* **Для кого:** Если хочешь включить VPN и забыть о нем.

**Ссылка для установки:**
`https://cdn.jsdelivr.net/gh/vasyakin/shadowrocket-rules@main/config/setup_stable.conf`

---

### 2. Режим "Only Blocked" 
**Логика:** Только конкретные списки заблокированных сайтов (из папки `/rules/proxy`) идут через прокси. **Весь остальной** интернет по умолчанию идет напрямую.
* **Для кого:** Если нужен доступ только к конкретным сервисам (Instagram, YouTube, ChatGPT), а всё остальное должно лететь через провайдера.

**Ссылка для установки:**
`https://cdn.jsdelivr.net/gh/vasyakin/shadowrocket-rules@main/config/setup_only_blocked.conf`

---

## 🛠 Структура правил (RULE-SET)

Правила разбиты на независимые модули для экономии ресурсов телефона и удобного редактирования:

* **⚡️ AI:** ChatGPT, Claude, Gemini, Grok.
* **📺 Streaming:** Netflix, Кинопоиск, HDRezka, Zetflix, Anime.
* **🎮 Games:** Supercell (Brawl Stars, CoC), Epic Games, Steam.
* **📱 Social:** Instagram, Facebook, X (Twitter), TikTok.
* **💬 Messengers:** Telegram, WhatsApp, Viber, Discord.
* **🎵 Music:** Spotify, SoundCloud, Mixcloud.
* **🏁 Sports:** Formula 1 (F1 TV & Live Timing).
* **🇷🇺 Direct RU:** Банки, Госуслуги, Яндекс, ВК, Почта.
* **🇨🇳 Direct CN:** Poizon (Dewu), Alipay, WeChat, Taobao.

---

## 🔄 Обновление
Все списки подгружаются через `RULE-SET`. 
1. Если вы измените файл в папке `/rules/`, Shadowrocket подтянет изменения автоматически.
2. Для принудительного обновления в приложении: **Config -> Нажать на конфиг -> Force Update**.

---
*Repo maintained by [vasyakin](https://github.com/MyNicknme)*
