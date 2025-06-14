# 🧠 Запуск нейросетей на слабом ПК — реально!

Многие думают, что нейросети вроде ChatGPT, Stable Diffusion или RVC можно запускать только на топовом железе. На деле — можно адаптировать их даже под **старые ноутбуки или ПК без GPU**.

---

## 🔸 Что можно запустить на слабом ПК?

| Нейросеть        | Да (CPU) | GPU (обязательно) | Есть облегчённые версии |
|------------------|----------|--------------------|--------------------------|
| LLaMA / Mistral  | ✅        | ❌                 | ✅ (GGUF, int4/int8)     |
| Stable Diffusion | ✅        | ⚠️ желательно       | ✅ (Lite-модели <2 ГБ)   |
| RVC (Voice Cloning) | ✅    | ❌                 | ✅                       |
| Whisper (STT)    | ✅        | ❌                 | ✅                       |

---

## 🔸 Где брать облегчённые модели?

- [HuggingFace.co](https://huggingface.co/) — фильтр по GGUF, quantized
- [TheBloke](https://huggingface.co/TheBloke) — лидер по конвертации моделей в GGUF
- [Civitai.com](https://civitai.com) — SD модели, есть ultra-lite
- [Ollama](https://ollama.com) — готовые образы для LLaMA, Gemma и т.д.

---

## 🔸 Что использовать для запуска?

### LLM (текстовые ИИ):
- **LM Studio** — простой интерфейс, работает на CPU
- **Ollama** — терминал+UI, оптимизирован для offline-LLM
- **Text Generation WebUI** — самый гибкий, но ресурсоёмкий

### Изображения (Stable Diffusion):
- **Stable Diffusion WebUI** — работает даже без GPU с CPU mode
- **InvokeAI** — лёгкая альтернатива WebUI
- **DiffusionBee** — под macOS / Windows

### Голос / Аудио:
- **RVC (Retrieval-Based Voice Conversion)** — для смены голоса
- **Whisper** — голос в текст (стенография)

---

## 🔸 Оптимизация слабого железа

- Увеличить pagefile/swap (мин. 8 ГБ)
- Временно отключить фоновые службы
- Использовать quantized модели (int4)
- Работать в offline-режиме, не загружая сеть

---

## 📎 Полезные ссылки

- https://github.com/ollama/ollama  
- https://github.com/oobabooga/text-generation-webui  
- https://github.com/RVC-Project/Retrieval-based-Voice-Conversion  
- https://github.com/AUTOMATIC1111/stable-diffusion-webui


🧰 Даже если у тебя только 4 ядра и 8 ГБ ОЗУ — ты всё ещё можешь запускать ИИ у себя, **без шпионства облаков и лагов браузера**.

🛠 Автор: @marselcomp
📡 Telegram-канал: @whatmarsel
"""
