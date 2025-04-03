# python-learning-by-week
基于chatgpt给出的python练习周计划打卡


---

## 🗓️ **第1周任务安排（共7天）**

### ✅ 学习目标：
- 掌握变量、数据类型、条件语句、循环等基本语法
- 熟悉列表、字典、元组、集合的用法
- 学会用控制结构编写小程序
- 输出第一个小项目 🛒

---

### 📅 **Day 1：环境搭建 + 第一个程序**
- 安装 Python、VSCode 或 Jupyter Notebook
- 运行第一个程序：`print("Hello, Python!")`
- 学习：变量、数据类型（int, float, str, bool）
  
📌练习：
```python
# 定义并打印各种类型变量
name = "Alice"
age = 25
height = 1.65
is_student = True
print(name, age, height, is_student)
```

---

### 📅 **Day 2：条件语句 & 输入输出**
- 学习 if / elif / else 语句
- 学习 input() 输入、print() 输出

📌练习：
```python
# 用户输入一个数字，判断它是正数、负数还是0
num = int(input("请输入一个数字："))
if num > 0:
    print("正数")
elif num < 0:
    print("负数")
else:
    print("零")
```

---

### 📅 **Day 3：循环结构**
- 学习 `for` 和 `while` 循环
- `range()` 的使用

📌练习：
```python
# 打印1到100内所有偶数
for i in range(1, 101):
    if i % 2 == 0:
        print(i)
```

---

### 📅 **Day 4：列表、字典、元组、集合**
- 学会增删查改、遍历列表
- 理解列表 vs 元组，字典 vs 集合的不同

📌练习：
```python
# 统计列表中每个元素出现的次数
fruits = ["apple", "banana", "apple", "orange", "banana"]
count_dict = {}
for fruit in fruits:
    count_dict[fruit] = count_dict.get(fruit, 0) + 1
print(count_dict)
```

---

### 📅 **Day 5：综合练习题（LeetCode or 牛客网）**
- ✨ 两数之和（列表+字典）【推荐题号：LeetCode #1】
- ✨ 判断回文字符串（字符串处理）
- ✨ 列表去重 & 排序

如果你需要题目中文链接，我也可以提供~

---

### 📅 **Day 6-7：小项目实战 - 购物清单管理器 🛒**

🛠️ 功能需求：
- 添加商品
- 删除商品
- 查看当前购物清单
- 输入 `exit` 后退出程序

📌 示例：
```python
shopping_list = []

while True:
    action = input("请输入操作（add/del/show/exit）：")
    if action == "add":
        item = input("添加商品：")
        shopping_list.append(item)
    elif action == "del":
        item = input("删除商品：")
        if item in shopping_list:
            shopping_list.remove(item)
    elif action == "show":
        print("购物清单：", shopping_list)
    elif action == "exit":
        break
```

---
