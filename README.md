# Roblox AI 🐢

The first project in the Roblox, showing the text2embedding model and the text classifier. As a bonus, there is the use of GPT-like models via the API.

**📺 [Watch the Video on YouTube!](https://youtu.be/I8dnvAJTnaA)**

---

## English

### 📦 Project Files
*   `RobloxAI_eng.rbxl`: English version.
*   `RobloxAI_ru.rbxl`: Russian version.

### ✨ Core Components
*   **🧠 Embedding Model:** A custom model to turn text into numbers (embeddings), using Word2Vec with symbols.
*   **🛡️ Toxicity Classifier:** A multilayer perceptron (MLP) to classify chat messages as safe/toxic.
*   **💬 Generative NPCs:** Integration with OpenAI & DeepInfra API for smart NPC dialogue, cheap and fast.

### ⚙️ Quick Setup

Before you start, you **must**:
1.  **Publish** the place (can be private).
2.  In `Game Settings > Security`, enable **`Studio Access to API Services`**.
3.  In `Game Settings > Security`, enable **`Allow HTTP Requests`**.

#### Training Your Models (Local AI)
The training process is sequential.
1.  Edit the dataset in `ServerScriptService > Emdeddings_Word2Vec`, then **Run** the game to train it.
2.  After it saves, **disable** the `Emdeddings_Word2Vec` script.
3.  Edit the dataset in `ServerScriptService > MLP_text` and **Run** to train the classifier.

#### Using Generative NPCs (External AI)
1.  Get your API key from [OpenAI](https://openai.com/) or [DeepInfra](https://deepinfra.com/).
2.  Select the `OpenAIChat` or `DeepInfra` ModuleScript. In the `Properties` window, add your key to the **`API_KEY` Attribute**.
3.  Enable the scripts and run the game.

### License
This project is licensed under GPLv3. For more information, see the [LICENSE](LICENSE).

---

## Русский

### 📦 Файлы Проекта
*   `RobloxAI_eng.rbxl`: Английская версия.
*   `RobloxAI_ru.rbxl`: Русская версия.

### ✨ Ключевые Компоненты
*   **🧠 Модель Обработки Текста (Эмбеддинги):** Кастомная модель для преобразования текста в числа (векторы), использующая Word2Vec с символами.
*   **🛡️ Классификатор Токсичности:** Многослойный перцептрон (MLP) для классификации сообщений в чате как безопасные/токсичные.
*   **💬 Генеративные NPC:** Интеграция с API OpenAI и DeepInfra для осмысленных диалогов NPC, дешёво и быстро.

### ⚙️ Быстрая Настройка

Перед началом вы **должны**:
1.  **Опубликовать** плейс (может быть приватным).
2.  В `Game Settings > Security` включите **`Studio Access to API Services`**.
3.  В `Game Settings > Security` включите **`Allow HTTP Requests`**.

#### Обучение ваших моделей (Локальный ИИ)
Процесс обучения последовательный.
1.  Отредактируйте датасет в `ServerScriptService > Emdeddings_Word2Vec`, затем **запустите (Run)** игру, чтобы обучить модель.
2.  После сохранения **отключите** скрипт `Emdeddings_Word2Vec`.
3.  Отредактируйте датасет в `ServerScriptService > MLP_text` и **запустите (Run)** игру, чтобы обучить классификатор.

#### Использование генеративных NPC (Внешний ИИ)
1.  Получите ваш API-ключ на [OpenAI](https://openai.com/) или [DeepInfra](https://deepinfra.com/).
2.  Выберите ModuleScript `OpenAIChat` или `DeepInfra`. В окне `Properties` добавьте ваш ключ в **атрибут `API_KEY`**.
3.  Включите скрипты и запустите игру.

### Лицензия
Этот проект лицензирован под GPLv3. Подробнее см. в файле [LICENSE](LICENSE).
