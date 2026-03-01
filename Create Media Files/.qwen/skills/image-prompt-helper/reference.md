# Reference: Критерии анализа и примеры промптов

## 📊 6 Критериев анализа изображений

### 1. Соответствие промпту (Prompt Accuracy)

**Что оценивать:**
- Все ли объекты из промпта присутствуют на изображении?
- Правильно ли переданы характеристики (порода, окрас, поза)?
- Соответствует ли окружение описанию?
- Передано ли настроение и атмосфера?

**Вопросы для анализа:**
- Какие элементы промпта упущены?
- Есть ли лишние детали, которых не было в промпте?
- Насколько точно интерпретирован запрос?

**Оценка:**
- **10/10** — Все элементы точно переданы
- **7-9/10** — Большинство элементов верно, мелкие неточности
- **4-6/10** — Половина элементов верна, есть существенные отклонения
- **1-3/10** — Изображение мало соответствует промпту

---

### 2. Композиция (Composition)

**Что оценивать:**
- Баланс элементов в кадре
- Наличие явного фокуса (главного объекта)
- Расположение объектов (правило третей, золотое сечение)
- Перспектива и глубина
- Направление взглядов и линий

**Вопросы для анализа:**
- Куда первым делом падает взгляд?
- Сбалансирована ли композиция или перевешена в одну сторону?
- Есть ли "воздух" вокруг объектов или всё слишком сжато?
- Работает ли перспектива?

**Оценка:**
- **10/10** — Идеальный баланс, явный фокус, профессиональная композиция
- **7-9/10** — Хорошая композиция с мелкими недочётами
- **4-6/10** — Композиция слабая, но терпимая
- **1-3/10** — Хаотичное расположение, нет фокуса

---

### 3. Цветовая палитра (Color Palette)

**Что оценивать:**
- Гармония цветов (сочетаются ли оттенки)
- Соответствие настроения палитре (тёплое = тёплые цвета)
- Наличие акцентов (выделяющиеся элементы)
- Баланс света и тени
- Отсутствие цветовых "шумов" (грязных оттенков)

**Вопросы для анализа:**
- Какие доминирующие цвета?
- Создают ли они нужное настроение?
- Есть ли цветовые диссонансы?
- Хорошо ли читается изображение в ч/б (проверка контраста)?

**Оценка:**
- **10/10** — Идеальная гармония, цвета усиливают настроение
- **7-9/10** — Хорошая палитра, мелкие недочёты
- **4-6/10** — Цвета работают, но без изысков
- **1-3/10** — Цветовой хаос, диссонирующие оттенки

---

### 4. Детализация (Detail Level)

**Что оценивать:**
- Проработка текстур (шерсть, кожа, ткань, природа)
- Чёткость мелких элементов (глаза, когти, листья)
- Отсутствие артефактов генерации (размытости, искажения)
- Глубина проработки фона и переднего плана

**Вопросы для анализа:**
- Видны ли отдельные шерстинки/волоски?
- Чёткие ли глаза (блики, зрачки, радужка)?
- Нет ли "пластикового" эффекта?
- Проработан ли фон или размыт?

**Оценка:**
- **10/10** — Безупречная детализация, видно каждую мелочь
- **7-9/10** — Хорошая детализация с мелкими недочётами
- **4-6/10** — Средняя детализация, некоторые элементы размыты
- **1-3/10** — Изображение "мыльное", детали упущены

---

### 5. Стиль (Style Consistency)

**Что оценивать:**
- Единый художественный стиль по всему изображению
- Соответствие стиля задумке (реализм, иллюстрация, акварель)
- Профессионализм исполнения
- Отсутствие стилевых конфликтов (например, фотореализм + мультяшность)

**Вопросы для анализа:**
- Какой стиль использован?
- Выдержан ли он от начала до конца?
- Выглядит ли профессионально или любительски?
- Соответствует ли стиль настроению промпта?

**Оценка:**
- **10/10** — Безупречный стиль, профессиональное исполнение
- **7-9/10** — Хороший стиль с мелкими недочётами
- **4-6/10** — Стиль есть, но с проблемами
- **1-3/10** — Стилевой хаос, разные элементы в разных стилях

---

### 6. Эмоциональный отклик (Emotional Impact)

**Что оценивать:**
- Какое настроение передаёт изображение?
- Вызывает ли оно эмоции (тёплые, ностальгические, вдохновляющие)?
- Запоминается ли изображение?
- Хочется ли на него смотреть дольше?

**Вопросы для анализа:**
- Что я чувствую, глядя на это изображение?
- Передаёт ли оно задуманное настроение?
- Зацепило ли оно меня лично?
- Какое из двух изображений сильнее воздействует?

**Оценка:**
- **10/10** — Сильное эмоциональное воздействие, "цепляет"
- **7-9/10** — Хорошее настроение, приятное изображение
- **4-6/10** — Нейтральное, не вызывает сильных эмоций
- **1-3/10** — Холодное, безэмоциональное

---

## 📝 Примеры промптов

### Пример 1: Дружба Смельчака и Генриха

**Короткий запрос:**
```
Две собаки дружат
```

**Улучшенный промпт:**
```
A heartwarming illustration of two best friend dogs: a silver-white labrador (Smelchak) with warm brown eyes and a black-and-tan german shepherd (Genrikh) with green eyes, standing side by side in a sunny meadow. The labrador has a joyful, optimistic expression while the german shepherd looks wise and protective. Soft golden hour lighting with warm peach and lavender tones. Natural retro illustration style, reminiscent of vintage storybook art. Detailed fur texture, gentle shadows, peaceful atmosphere. Colors: earthy browns, grassy greens, soft lilac accents. Avoid cold office colors. Mood: friendship, loyalty, warmth, nostalgia. Professional digital illustration, high quality.
```

**Что добавлено:**
- Персонажи: породы, окрас, имена, выражения
- Окружение: солнечная поляна
- Освещение: золотой час
- Стиль: природный ретро, винтажная иллюстрация
- Цвета: древесные, травянистые, лиловые (предпочтения проекта)
- Настроение: дружба, верность, тепло

---

### Пример 2: Щенок Смельчак

**Короткий запрос:**
```
Щенок лабрадора играет
```

**Улучшенный промпт:**
```
An adorable silver-white labrador puppy (young Smelchak) playing in a spring garden, jumping joyfully with tongue out and bright brown eyes full of curiosity. Soft morning sunlight filtering through fresh green leaves. Fallen cherry blossom petals on the grass. Watercolor illustration style with soft edges and dreamy atmosphere. Pastel color palette: light greens, soft pinks, warm cream tones. Close-up perspective at puppy's eye level. Mood: innocence, joy, discovery, childhood wonder. Detailed fur texture, expressive face. Natural retro aesthetic, avoiding cold modern colors. Professional children's book illustration quality.
```

**Что добавлено:**
- Персонаж: щенок, конкретная порода и окрас
- Действие: прыгает радостно, язык наружу
- Окружение: весенний сад, цветущая вишня
- Освещение: утреннее солнце
- Стиль: акварель, мягкие края
- Цвета: пастельные, тёплые
- Ракурс: на уровне глаз щенка
- Настроение: невинность, радость, детское чудо

---

### Пример 3: Генрих-философ

**Короткий запрос:**
```
Немецкая овчарка мудрая
```

**Улучшенный промпт:**
```
A portrait of a wise german shepherd (Genrikh) with deep green eyes and thick black-and-tan fur, sitting calmly in an autumn forest. Golden and orange leaves falling gently around. The dog has a thoughtful, slightly melancholic expression with warm, sad eyes that tell a story of hardship and wisdom. Soft diffused lighting through tree canopy. Oil painting style with rich textures and deep colors. Color palette: warm browns, burnt orange, deep green, golden yellow. Medium close-up, eye level perspective. Mood: wisdom, melancholy, resilience, quiet strength. Detailed fur texture, expressive eyes with subtle reflections. Natural retro style, avoiding cold tones. Professional fine art quality.
```

**Что добавлено:**
- Персонаж: конкретная внешность Генриха
- Выражение: задумчивое, меланхоличное, мудрое
- Окружение: осенний лес, падающие листья
- Стиль: масляная живопись, богатые текстуры
- Цвета: тёплые коричневые, оранжевые, глубокие зелёные
- Настроение: мудрость, меланхолия, стойкость

---

### Пример 4: Пожарный Смельчак

**Короткий запрос:**
```
Собака спасатель на пожаре
```

**Улучшенный промпт:**
```
A heroic silver-white labrador (Smelchak as a rescue dog) in action, wearing a red rescue vest, emerging from a smoky building with determination in his brown eyes. Dramatic lighting with orange and red fire glow contrasting against dark smoke. Dynamic composition with diagonal lines suggesting movement and urgency. Realistic digital painting style with detailed fur texture and atmospheric effects. Color palette: warm oranges, deep reds, dark grays, with the white labrador standing out as a beacon of hope. Low angle perspective to emphasize heroism. Mood: courage, determination, hope in darkness. Professional action illustration, high detail.
```

**Что добавлено:**
- Персонаж: Смельчак в спасательном жилете
- Действие: выходит из здания с решимостью
- Окружение: дым, огонь
- Освещение: драматичное, оранжево-красное
- Стиль: реалистичная цифровая живопись
- Композиция: динамичная, диагональные линии
- Настроение: мужество, решимость, надежда

---

## 🎨 Шаблоны промптов для проекта "Собачья мудрость"

### Шаблон 1: Портрет персонажа

```
A [style] portrait of [dog name], a [breed] with [coat color] fur and [eye color] eyes. The dog has a [expression] expression, conveying [emotion]. [Lighting type] lighting from [direction]. [Background description]. Color palette: [colors matching project preferences]. Mood: [mood words]. [Style details], professional quality, detailed fur texture.
```

### Шаблон 2: Сцена дружбы

```
A heartwarming [style] scene of [dog 1] and [dog 2] [action] together in [location]. [Dog 1 description] on the [side], [dog 2 description] on the [side]. [Lighting description] creating [atmosphere]. [Background elements]. Colors: [warm/earthly tones]. Mood: [friendship/loyalty/joy]. [Style specifics], avoiding cold colors. Professional illustration quality.
```

### Шаблон 3: Приключенческая сцена

```
A dynamic [style] illustration of [dog name] [action verb] through [environment]. The [breed] has [expression] with [details]. Dramatic [lighting type] with [color] highlights. [Foreground elements], [background elements]. Composition: [perspective and angle]. Color palette: [adventurous colors]. Mood: [excitement/courage/determination]. [Style details], high detail, professional quality.
```

### Шаблон 4: Медитативная/философская сцена

```
A contemplative [style] scene of [dog name] [calm action] in [peaceful location]. The [breed] has a [thoughtful expression] with [eye details]. Soft [lighting type] creating [gentle atmosphere]. [Natural elements like leaves, water, grass]. Muted color palette: [soft earthy tones]. Mood: [peace/wisdom/reflection]. [Style specifics], dreamy quality, detailed textures.
```

---

## ⚡ Быстрые советы по улучшению

### Добавь конкретики:
- ❌ "собака" → ✅ "серебристо-белый лабрадор с карими глазами"
- ❌ "на улице" → ✅ "на солнечной поляне в весеннем лесу"
- ❌ "красиво" → ✅ "в стиле винтажной книжной иллюстрации"

### Добавь настроения:
- ❌ "весело" → ✅ "радостно, с беззаботностью щенка"
- ❌ "грустно" → ✅ "с тихой меланхолией и мудростью в глазах"

### Добавь света:
- ❌ "освещение" → ✅ "мягкий свет золотого часа, тёплые блики"
- ❌ "тени" → ✅ "нежные тени, создающие глубину"

### Добавь стиля:
- ❌ "рисунок" → ✅ "акварель с мягкими краями и мечтательной атмосферой"
- ❌ "картинка" → ✅ "реалистичная цифровая живопись с детализированной шерстью"

---

*Документ является частью скилла Image Prompt Helper. Последнее обновление: 28 февраля 2026 г.*
