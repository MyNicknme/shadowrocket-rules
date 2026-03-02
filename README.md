# 🚀 Shadowrocket Config & Auto-Updating Rules

Набор оптимизированных правил для **Shadowrocket (iOS)**, разделенных по сервисам.  
Правила обновляются автоматически через `RULE-SET` (без ручного редактирования на телефоне).

---

## 📥 Варианты установки

### 1) Режим **VPN-by-default** (рекомендуемый)
**Логика:** важные сервисы (банки/госуслуги/Apple/China) идут **напрямую (DIRECT)**.  
Всё остальное — **через прокси (PROXY)**.

**Для кого:** если хочешь включить VPN и забыть о нём.

✅ **Ссылка для установки (ветка main):**

https://cdn.jsdelivr.net/gh/MyNicknme/shadowrocket-rules@main/config/VPN-by-default.conf

✅ **Если вы меняли структуру конфига (добавляли новые RULE-SET):**  
используйте permalink на конкретный коммит (или переустановите конфиг заново).

https://cdn.jsdelivr.net/gh/MyNicknme/shadowrocket-rules@<COMMIT_HASH>/config/VPN-by-default.conf

---

### 2) Режим **Only Blocked**
**Логика:** через прокси идут только сервисы из папки `/rules/proxy`.  
Весь остальной интернет по умолчанию идёт напрямую.

**Для кого:** если нужен доступ только к конкретным сервисам (Instagram / YouTube / ChatGPT), а остальное — напрямую.

✅ **Ссылка для установки:**

https://cdn.jsdelivr.net/gh/MyNicknme/shadowrocket-rules@main/config/setup_only_blocked.conf

---

## 🛠 Структура правил (RULE-SET)

Правила разбиты на независимые модули — так проще поддерживать и меньше нагрузки на телефон:

- **⚡️ AI:** ChatGPT, Claude, Gemini, Grok, Copilot, DeepL, ElevenLabs и т.д.
- **📺 Streaming:** Netflix, Rezka, LostFilm, Zetflix, Anime и т.п. *(YouTube — отдельным файлом)*
- **📱 Social:** Instagram/Facebook, X (Twitter), TikTok
- **💬 Messengers:** Telegram, WhatsApp, Viber, Discord
- **🎵 Music:** Spotify, SoundCloud, Mixcloud
- **🏁 Sports:** Formula 1 (F1 TV & Live Timing)
- **🇷🇺 Direct RU:** банки, Госуслуги, Яндекс, ВК, Почта и т.п.
- **🇨🇳 Direct CN:** Poizon (Dewu), Alipay, WeChat, Taobao и т.п.
- **🧱 Block:** реклама/трекеры (`ads.list`)

---

## 🔄 Обновление

### Как обновляются правила
- Файлы в `/rules/*.list` загружаются через `RULE-SET` и обновляются автоматически.
- Для принудительного обновления:  
  **Config → выбрать конфиг → Force Update / Update**.

### Важное про обновление `.conf`
Shadowrocket не всегда “пересобирает” конфиг, если вы добавили новые `RULE-SET`.  
Если вы обновили **структуру** конфига (добавили новые списки), используйте:
- permalink на commit (`@<COMMIT_HASH>`)  
или переустановите конфиг по ссылке заново.

---

*Repo maintained by **MyNicknme***
