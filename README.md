graph TD
    A[Событие OnManagerTreePrerender] --> B{Пользователь = админ?}
    B -- Да --> C[Чтение конфига use_modx_popup]
    B -- Нет --> D[Выход]
    C --> E[Рендер tree-button.blade.php]
    E --> F[Вывод HTML в дерево]
