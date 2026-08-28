# Coffee Shop Website — Design Specification

## 1. Concept & Vision

Уютный сайт кофейни с тёплой атмосферой. Дизайн вызывает ощущение утреннего кофе и приятного времяпровождения. Минимализм с акцентом на качественные фото и элегантную типографику.

## 2. Design Language

### Aesthetic Direction
Скандинавский минимализм с тёплыми кофейными тонами. Чистые линии, много воздуха, акцент на контенте.

### Color Palette
- **Primary:** `#5D4037` (тёмный кофе)
- **Secondary:** `#8D6E63` (молочный шоколад)
- **Accent:** `#FFAB91` (персиковый)
- **Background:** `#FFF8F0` (крем)
- **Text:** `#3E2723` (эспрессо)
- **Light:** `#EFEBE9` (светлый беж)

### Typography
- **Headings:** 'Playfair Display', Georgia, serif
- **Body:** 'Inter', -apple-system, sans-serif

### Spatial System
- Base unit: 8px
- Section padding: 80px vertical
- Container max-width: 1200px

### Motion Philosophy
- Плавные fade-in при скролле (opacity 0→1, 600ms ease-out)
- Hover на карточках: translateY(-8px), 300ms
- Кнопки: scale(1.02), 200ms

## 3. Layout & Structure

### Pages
1. **Home** — герой-секция, о нас, меню (хиты), отзывы, контакты
2. **Menu** — полный каталог напитков и десертов с фильтрами
3. **About** — история кофейни, команда
4. **Contact** — карта, форма обратной связи, часы работы

### Sections (Home)
- Hero: full-height с фоновым изображением и слоганом
- About Preview: 2 колонки (текст + фото)
- Popular Menu: сетка карточек 3 колонки
- Testimonials: слайдер отзывов
- Contact CTA: баннер с призывом
- Footer: навигация, соцсети, копирайт

### Responsive Strategy
- Desktop: 1200px+ (полная сетка)
- Tablet: 768px-1199px (2 колонки)
- Mobile: <768px (1 колонка, бургер-меню)

## 4. Features & Interactions

### Navigation
- Фиксированная шапка, становится компактнее при скролле
- Плавный скролл к секциям
- Мобильное меню: slide-in справа

### Menu Cards
- Hover: подъём + тень
- Click: модальное окно с описанием
- Цена, название, теги (хит, новый, вегетарианский)

### Contact Form
- Поля: имя, email, телефон, сообщение
- Валидация в реальном времени
- Состояние загрузки при отправке
- Toast-уведомление об успехе/ошибке

### Hero
- Параллакс-эффект на фоне
- Анимированный заголовок

## 5. Component Inventory

### Button
- Primary: bg `#5D4037`, text white, rounded 8px
- Hover: bg `#4E342E`, scale 1.02
- Disabled: opacity 0.5, cursor not-allowed

### Card (Menu Item)
- White bg, rounded 16px, shadow
- Image top, content padding 24px
- Tag badge absolute top-right

### Navigation Link
- Default: `#3E2723`
- Hover: `#5D4037`, underline offset animation
- Active: `#5D4037`, bold

### Input Field
- Border: 1px `#D7CCC8`
- Focus: border `#5D4037`, shadow
- Error: border `#E53935`, error message below

### Section Title
- Playfair Display, 48px desktop / 32px mobile
- Subtitle: Inter, 18px, `#8D6E63`

## 6. Technical Approach

- **Stack:** HTML5, CSS3 (vanilla), JavaScript (ES6+)
- **No frameworks** — чистая реализация для портфолио
- **CSS:** Custom properties, Flexbox, Grid
- **JS:** Modules, async/await, IntersectionObserver for animations
- **Assets:** Placeholder images from picsum/unsplash
- **Icons:** Inline SVG
