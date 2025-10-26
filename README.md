import random

def guess_number():
    # Компьютер загадывает число
    number = random.randint(1, 100)
    attempts = 0
    print("Я загадал число от 1 до 100. Попробуй угадать!")

    while True:
        try:
            # Запрашиваем число у игрока
            guess = int(input("Введи число: "))
            attempts += 1

            # Проверяем, угадал ли игрок
            if guess < number:
                print("Слишком мало
