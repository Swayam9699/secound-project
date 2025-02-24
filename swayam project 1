# Simple To-Do List Application

# List to store tasks
tasks = []

def display_tasks():
    if not tasks:
        print("Your To-Do List is empty!")
    else:
        print("\nYour To-Do List:")
        for idx, task in enumerate(tasks, start=1):
            print(f"{idx}. {task}")

def add_task():
    task = input("Enter a new task: ")
    tasks.append(task)
    print(f"Task '{task}' added!")

def remove_task():
    display_tasks()
    try:
        task_num = int(input("Enter the task number you want to remove: "))
        if 1 <= task_num <= len(tasks):
            removed_task = tasks.pop(task_num - 1)
            print(f"Task '{removed_task}' removed!")
        else:
            print("Invalid task number!")
    except ValueError:
        print("Please enter a valid number.")

def mark_completed():
    display_tasks()
    try:
        task_num = int(input("Enter the task number you want to mark as completed: "))
        if 1 <= task_num <= len(tasks):
            tasks[task_num - 1] += " (Completed)"
            print(f"Task '{tasks[task_num - 1]}' marked as completed!")
        else:
            print("Invalid task number!")
    except ValueError:
        print("Please enter a valid number.")

def main():
    while True:
        print("\nTo-Do List Menu:")
        print("1. View tasks")
        print("2. Add task")
        print("3. Remove task")
        print("4. Mark task as completed")
        print("5. Exit")

        choice = input("Choose an option: ")

        if choice == '1':
            display_tasks()
        elif choice == '2':
            add_task()
        elif choice == '3':
            remove_task()
        elif choice == '4':
            mark_completed()
        elif choice == '5':
            print("Goodbye!")
            break
        else:
            print("Invalid choice! Please select a valid option.")

if __name__ == "__main__":
    main()
