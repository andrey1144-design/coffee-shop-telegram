# Coffee Shop Website — Agent Instructions

## Project Overview
Создание сайта для кофейни "Coffee & Dreams" — уютная кофейня с авторскими напитками и домашней атмосферой.

## Workflow

### Phase 1: Setup
1. Создать структуру проекта:
   ```
   /coffee-shop
     /assets
       /images
       /css
         style.css
       /js
         main.js
     index.html
     menu.html
     about.html
     contact.html
   ```

### Phase 2: Implementation

#### HTML Pages
- **index.html** — главная страница со всеми секциями
- **menu.html** — полный каталог меню
- **about.html** — история и команда
- **contact.html** — контакты и форма

#### CSS (assets/css/style.css)
1. CSS Variables для дизайн-системы (colors, typography, spacing)
2. Reset и base styles
3. Layout utilities (container, grid, flex)
4. Components (buttons, cards, inputs, navigation)
5. Section-specific styles
6. Responsive breakpoints
7. Animations (fade-in, hover effects)
8. Utility classes

#### JavaScript (assets/js/main.js)
1. Mobile menu toggle
2. Smooth scroll navigation
3. Header compact on scroll
4. Scroll animations (IntersectionObserver)
5. Form validation and submission
6. Menu filtering
7. Modal functionality

### Phase 3: Content

#### Menu Items (at least 12)
- **Coffee:** Espresso, Americano, Cappuccino, Latte, Flat White, Mocha
- **Non-coffee:** Matcha Latte, Hot Chocolate, Chai Latte
- **Desserts:** Cheesecake, Tiramisu, Croissant, Brownie

#### About Content
- История основания (2020 год)
- Миссия: "Каждая чашка — как первый глоток утреннего кофе"
- Команда: 2 бариста, 1 менеджер

#### Testimonials (3 штуки)
- Реалистичные отзывы гостей

### Phase 4: Polish
1. Проверить все hover-эффекты
2. Убедиться в работоспособности навигации
3. Проверить адаптивность
4. Добавить favicon
5. Meta tags для SEO

## Quality Checklist
- [ ] Все ссылки работают
- [ ] Все формы валидируются
- [ ] Мобильное меню открывается/закрывается
- [ ] Анимации плавные (60fps)
- [ ] Нет console errors
- [ ] Файл style.css < 500 строк ( организованный)
- [ ] JS использует современный ES6+
