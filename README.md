# hw100925.py

## ДЗ
    Курс: AI+Python 
    Модуль 12. Структури даних 
    Тема: Зв’язні списки. 
    Частина 1
     Завдання 1 
    Використовуючи класи з практичної реалізуйте клас Shop з 
    трьома чергами до кас. Кожна черга реалізується через 
    двозв’язний список 
    Атрибути 
     queue1, queue2, queue3 – черги до кас 
    Методи 
     add_buyer(name, idx) – додає покупця в кінець черги 
    номер idx 
     serve_buyer(idx) – обслуговує покупця з черги 
    idx(вивести повідомлення та видалити покупця з черги) 
    Якщо черга стала порожньою, то викликати _reorder(idx) 
     _reorder(idx) – з усіх черг останній покупець переходить 
    в чергу з номером idx 
     display_info() – виводить на екран 3 черги 
    Посилання на код 
    # Приклад використання 
    shop = Shop() 
    shop.add_buyer("Олег", 1) 
    shop.add_buyer("Марина", 2) 
    shop.add_buyer("Марія", 2) 
    shop.add_buyer("Андрій", 3) 
    shop.add_buyer("Ірина", 1) 
    shop.add_buyer("Василь", 2) 
    shop.add_buyer("Тетяна", 3) 
    shop.add_buyer("Сергій", 3) 
    shop.add_buyer("Анна", 3) 
    print("Черги:") 
    shop. display_info() 
    shop.serve_buyer(1) 
    shop.serve_buyer(2) 
    shop.serve_buyer(3) 
    print("Після обслуговування покупців:") 
    shop. display_info() 
    shop.serve_buyer(1) 
    print("Покупці перейшли до вільної каси:") 
    shop. display_info()
