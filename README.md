# ✅ Mattermost To-Do Bot Commands(Spec Draft)

Welcome to your To-Do Bot! 🚀 Below is the complete guide to all the bot commands, helping you manage your tasks efficiently.

---

## 1️⃣ **Basic Task Management**

### Add a Task
```shell
/todo add [Task Description]
```
**Example:**  
`/todo add Submit quarterly report`

### Mark a Task as Done
```shell
/todo done [Task ID]
```
**Example:**  
`/todo done 3`

### Delete a Task
```shell
/todo delete [Task ID]
```
**Example:**  
`/todo delete 5`

### List All Tasks
```shell
/todo list
```
- Displays all tasks with their statuses, priorities, tags, and due dates.

### Clear All Completed Tasks
```shell
/todo clear
```
- Removes all tasks marked as done/completed.

---

## 2️⃣ **Task Prioritization**

### Set Priority for a Task
```shell
/todo priority [Task ID] [high/medium/low]
```
**Example:**  
`/todo priority 7 high`

### List Tasks by Priority
```shell
/todo list priority:[high/medium/low]
```
**Example:**  
`/todo list priority:high`

---

## 3️⃣ **Due Dates and Reminders**

### Set Due Date for a Task
```shell
/todo add [Task Description] due:[YYYY-MM-DD HH:mm]
```
**Example:**  
`/todo add Submit project proposal due:2023-10-25 14:00`

### Edit Due Date for a Task
```shell
/todo edit due [Task ID] [YYYY-MM-DD HH:mm]
```
**Example:**  
`/todo edit due 4 2023-10-30 09:00`

### List Tasks with Upcoming Deadlines
```shell
/todo list upcoming
```
**Example Output:**  
`2 Tasks due in the next 7 days!`

### Enable/Disable Reminders
```shell
/todo reminder [enable/disable]
```
**Example:**  
`/todo reminder enable`

---

## 4️⃣ **Task Tags**

### Add Tags to a Task
```shell
/todo tag [Task ID] #[tag1] #[tag2]
```
**Example:**  
`/todo tag 6 #work #highpriority`

### Filter Tasks by Tag
```shell
/todo list tag:[#tag_name]
```
**Example:**  
`/todo list tag:#work`

### Remove a Tag from a Task
```shell
/todo tag remove [Task ID] #[tag_name]
```
**Example:**  
`/todo tag remove 6 #highpriority`

---

## 5️⃣ **General Query and Search Commands**

### View a Specific Task
```shell
/todo view [Task ID]
```
**Example:**  
`/todo view 2`

### Search Tasks by Keyword
```shell
/todo search "keyword"
```
**Example:**  
`/todo search "submit"`

### Search Overdue Tasks
```shell
/todo list overdue
```
- Displays tasks whose deadlines have passed.

---

## Bonus: **Shortcut Commands**

For better usability, you can use shortcuts for common commands. For example:
- `/td add` instead of `/todo add`
- `/td list` instead of `/todo list`
- `/td tag` instead of `/todo tag`

**Shortcut Example:**  
`/td add Complete documentation draft`

---

## 🎯 **Command Example Workflow**

1. **Add a Task with Priority and Due Date:**  
   ```shell
   /todo add Complete presentation slides priority:high due:2023-10-20 16:00
   ```

2. **Add Tags:**  
   ```shell
   /todo tag 3 #work #urgent
   ```

3. **View Tasks with Filters:**  
   ```shell
   /todo list priority:high tag:#urgent upcoming
   ```

4. **Mark as Done:**  
   ```shell
   /todo done 3
   ```

---

Now you're ready to organize your tasks like a pro! 🎉 Happy productivity! ☑️
