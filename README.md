# SounKey-v3.0


Профессиональный навигационный комплекс для CS2, полностью нивелирующий задержки системы саб-тиков и предоставляющий функционал Snap Tap (SOCD) на программном уровне. Идеально подходит для KZ, Surf, Bhop и соревновательного режима.

github.com
GitHub - Solduramigopmo/CS2-De-subtick-Null-Binds-Snap-Tap-Turn
Contribute to Solduramigopmo/CS2-De-subtick-Null-Binds-Snap-Tap-Turn development by creating an account on GitHub.
github.com
Если вам понравилось - прошу поставить звезду на репозиторий.
Хорошего всем вечера!

---

## Технический функционал (De-Subtick)

Конфиг перерабатывает механику движений, привязывая каждое действие к тику сервера для максимальной точности.

### Прыжки и Джамп-баги
* **Long-Jump & Crouch-Jump:**
* `+lj` / `+ldj` — 100% автоматический Long-Crouch-Jump. Работает передом и задом без движения мыши.
* `+cj` — Автоматический Crouch-Jump во все 4 стороны.
* **Jump-Bugs:**
* `+scj` — Улучшенный полуавтоматический Scroll Jump-Bug.
* `bsjb_w` — Автоматический скролл-вариант для Long-Mini-Jump и Long-Crouch-Jump.
* **Mini-Jumps:**
* `+laj` — Автоматический Long-Mini-Jump или полуавтоматический Jump-Bug.

### Ладдеры и Данвари
* **Ladder-Tech:**
* `setup-lj_l` / `setup-lj_r` — Сброс оффсета (прыжок) для ладдеров.
* `+mbwd` — Полностью автоматический сброс оффсета для всех действий.
* **Danwari:**
* `+dnv_p` — Полуавтоматический 100% Данвари (любой стороной, ~9.62u).
* `+dnv_h` — Автоматический 100% Данвари (все действия передом).

### Стрейфы и Повороты
* **Null Binds (Snap Tap):**
* `+a` / `+d` и `+w` / `+s` — Исключают одновременное нажатие противоположных клавиш. Последнее нажатое направление всегда в приоритете.
* **Half Sideways (HSW):**
* `+mhsw_fl` / `+mhsw_bl` — Диагональные стрейфы с интегрированными нуллами.
* **Turn Binds (CS:GO Style):**
* `+tmlwd` / `+tmrwd` — Повороты по Yaw (до 300°) и Pitch (до 45°) с поддержкой нуллов.

---

## Утилиты и Визуал
* **Jumpstats Color:** Полная кастомизация цвета консоли (более 4 млрд цветов через `log_color`).
* **Noclip Hold:** `+nc` — Полет на удержание клавиши.
* **Quick Spec:** `+spec` — Мгновенный переход в наблюдатели (для Cybershoke/CS2KZ).
* **Flat Sens:** `togglesens_vert` — Отключение вертикальной оси мыши.

---

## Установка и Запуск

1. Распакуйте папку `movement_config` в:
`...\Steam\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg\`
2. **ВАЖНО:** Перенесите файлы `autoexec_movement.cfg` и `.vtest` из папки `movement_config` в корень `cfg`.
3. Добавьте в **параметры запуска Steam**:
```text
+exec "autoexec_movement.cfg" +alias "8CfyMR" -disable_workshop_command_filtering -testscript_inline "Test_Run ../../csgo/cfg/.vtest"
```

### Почему это важно?
- `-testscript_inline` запускает цикл через `.vtest`, что позволяет конфигу работать **каждый тик**.
- `-disable_workshop_command_filtering` разрешает использование продвинутых алиасов.

## Настройка
Назначение клавиш происходит в файле: `movement_config/core/settings.cfg`.
Все параметры сопровождены подробными комментариями на русском языке.
