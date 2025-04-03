```markdown
# 📘 Python Day 1 学习总结

## 🎯 学习目标

- 熟悉 Python 的基础语法
- 掌握变量、数据类型、输入输出、条件判断
- 学会定义函数、处理错误
- 完成第一个小项目：“字母清洗器”

---

## 📚 今日学习内容

### 1️⃣ 变量与数据类型

```python
name = "Alice"          # str
age = 25                # int
height = 1.65           # float
is_student = True       # bool
```

查看变量类型：

```python
print(type(name))  # <class 'str'>
```

---

### 2️⃣ 用户输入与类型转换

```python
user_input = input("请输入一个数字：")
num = int(user_input)
print(num, type(num))
```

异常处理版本：

```python
def safe_to_int(s):
    try:
        return int(s)
    except ValueError:
        return "输入错误"
```

---

### 3️⃣ 条件判断 if / else

```python
if guess == answer:
    print("你猜对了！")
else:
    print(f"你猜错了，正确答案是 {answer}")
```

---

### 4️⃣ 函数定义与调用

```python
def greet(name):
    print(f"Hello, {name}!")

greet("Alice")
```

---

### 5️⃣ 字符串处理方法

```python
s = " Hello, World!123 "
s = s.lower()            # 转小写
s = s.strip()            # 去空格
s.isalpha()              # 判断是否为纯字母
```

---

## 🛠️ 小项目：字母清洗器

### 🎯 功能：
接收用户输入的一段字符串，去除其中非字母字符，输出清洗后的结果。

---

### ✅ 项目代码

```python
def clean_letters(text):
    clean_text = ''
    for char in text:
        if char.isalpha():
            clean_text += char
    return clean_text

text = input("Please enter a sentence: ")
text = text.lower()
print(clean_letters(text))
```

---

### 🧪 示例

**输入：**
```
Hello, Python! 123 😊
```

**输出：**
```
hellopython
```

---

## ✅ 今日收获

- 掌握了 Python 中变量、输入、判断、函数、异常等基础语法
- 练习了从逻辑到代码实现的完整过程
- 能独立完成一个功能性小项目
- 对写代码的结构感有初步认知

---

📌 文件建议保存为：  
`/week1/day1_summary.md`  
或  
放在项目根目录的 `README.md` 中作为学习日志

---
