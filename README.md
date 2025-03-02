# ✅ Mattermost To-Do Bot Commands(Spec Draft)

Welcome to your To-Do Bot! This is a n8n workflow integrated mattermost slash command to record your to-dos.
🚀 Below is the complete guide to all the bot commands, helping you manage your tasks efficiently.

---

## 1️⃣ **Basic Task Management**

### Add a Task
```shell
/todo-add [Task Description]
```
**Example:**  
`/todo-add Submit quarterly report`

### Mark a Task as Done
```shell
/todo-done [Task ID]
```
**Example:**  
`/todo-done 3`

### Delete a Task(Coming Soon)
```shell
/todo-delete [Task ID]
```
**Example:**  
`/todo-delete 5`

### List All Tasks
```shell
/todo-list
```
- Displays all tasks with their statuses, priorities, tags, and due dates.
- Default to list all undone todos


- use below to list all status todos
```shell
/todo-list all
```

### Clear All Completed Tasks(Coming Soon)
```shell
/todo-clear
```
- Removes all tasks marked as done/completed.

---

## 2️⃣ **Task Prioritization**

### Set Priority for a Task(Coming Soon)
```shell
/todo-priority [Task ID] [high/medium/low]
```
**Example:**  
`/todo-priority 7 high`

### List Tasks by Priority(Coming Soon)
```shell
/todo-list priority:[high/medium/low]
```
**Example:**  
`/todo-list priority:high`

---

## 3️⃣ **Due Dates and Reminders**(Coming Soon)

### Set Due Date for a Task(Coming Soon)
```shell
/todo-add [Task Description] due:[YYYY-MM-DD HH:mm]
```
**Example:**  
`/todo-add Submit project proposal due:2023-10-25 14:00`

### Edit Due Date for a Task(Coming Soon)
```shell
/todo-due [Task ID] [YYYY-MM-DD HH:mm]
```
**Example:**  
`/todo-due 4 2023-10-30 09:00`

### Enable/Disable Reminders(Coming Soon)
```shell
/todo-reminder [enable/disable]
```
**Example:**  
`/todo-reminder enable`

---

## 4️⃣ **Task Tags**

### Add Tags to a Task(Coming Soon)
```shell
/todo-tag [Task ID] #[tag1] #[tag2]
```
**Example:**  
`/todo-tag 6 #work #highpriority`

### Filter Tasks by Tag(Coming Soon)
```shell
/todo-list tag:[#tag_name]
```
**Example:**  
`/todo-list tag:#work`

### Remove a Tag from a Task(Coming Soon)
```shell
/todo-tag remove [Task ID] #[tag_name]
```
**Example:**  
`/todo-tag remove 6 #highpriority`

---

## 🎯 **Command Example Workflow**

1. **Add a Task with Priority and Due Date:**  
   ```shell
   /todo-add Complete presentation slides priority:high due:2023-10-20 16:00
   ```

2. **Add Tags:**  
   ```shell
   /todo-tag 3 #work #urgent
   ```

3. **View Tasks with Filters:**  
   ```shell
   /todo-list priority:high tag:#urgent
   ```

4. **Mark as Done:**  
   ```shell
   /todo-done 3
   ```

---

Now you're ready to organize your tasks like a pro! 🎉 Happy productivity! ☑️
