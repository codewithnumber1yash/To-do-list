# To-do-list
def show_task(tasks)
if not tasks:
  print("No tasks yet.")
else:
  print("\nYour To-do list")
  for i,task in enumerate(tasks, 1):
    print(f"{i}. {task}")

def ass_task(tasks):
    task =input("Enter a new task:").strip()
    if task:
      task.append(task)
      print("task addwd.")
    else:
      print("Task cannot be empty.")
def update_task(tasks):
    show_tasks(tasks)
    if tasks:
      try:
          num = imt(input("ENter task number to update: "))
          if 1 <= num <= len(tasks):
            new_task = input("Enter the updated task:").strip()
            if new_task:
              tasks[num -1] = new_task
              print("Task updated.")
            else:
              print("task cannot be empty.")
          else:
            print("invalid task number.")
    except ValueError:
        print("Please enterr a valid number.")

  def main()
    tasks =[]
    whileTrue:
      print("\nMenu:")
      print("1. Show tasks")
      print("2. Add task")
      print("3. Update task")
      print("4. Exit")
      choice = input ("choose an option:")
      if choice =='1':
        show_tasks(tasks)
      elif choice == '2':
        add_tasks(tasks)
      elif choice == '3':
        update_task(tasks)
      elif choice == '4':
        print("Goodbye!")
        break
      else:
        print("Invalid Choice. Try again.")

if __name__ == "__main__":
  main()
      
