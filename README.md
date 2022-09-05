# attempt
today = []
tomorrow = [] 
other = []

run = True

while run:
  command = input("Введите команду: ")
  if command == "help":
    print(HELP)
  elif command == "show":
    print("today", today, "tomorrow", tomorrow, "other", other)
  elif command == "add":
    task = input("Введите название задачи: ")
    date = input("Введите дату выполнения задачи: ")
    date1 = "Сегодня"
    date2 = "Завтра"
    if date == date1:
     today.append(task)
    elif date == date2:
      tomorrow.append(task)
    else:
      other.append(task)
    print("Задача добавлена")
  elif command == "exit":
    print ("Спасибо за использование!До свидания!")
    break
  else: 
    print("Неизвестная команда. До свидания")
    break
