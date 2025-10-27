# Простий калькулятор

def calculator():
    print("Простий калькулятор")
    print("Оберіть операцію:")
    print("1. Додавання (+)")
    print("2. Віднімання (-)")
    print("3. Множення (*)")
    print("4. Ділення (/)")

    choice = input("Введіть номер операції (1/2/3/4): ")

    num1 = float(input("Введіть перше число: "))
    num2 = float(input("Введіть друге число: "))

    if choice == '1':
        print(f"Результат: {num1} + {num2} = {num1 + num2}")
    elif choice == '2':
        print(f"Результат: {num1} - {num2} = {num1 - num2}")
    elif choice == '3':
        print(f"Результат: {num1} * {num2} = {num1 * num2}")
    elif choice == '4':
        if num2 != 0:
            print(f"Результат: {num1} / {num2} = {num1 / num2}")
        else:
            print("Помилка: ділення на нуль!")
    else:
        print("Неправильний вибір операції!")

# Запуск програми
calculator()

