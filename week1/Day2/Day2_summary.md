当然可以！Day 2 是你迈入「Python 控制结构」的关键阶段 💡  
下面是为你整理的 **Day 2 知识点清单**，搭配你将要刷的 LeetCode 题，覆盖所有你需要掌握的重点内容 ✅

---

# 📘 Day 2 知识点：循环与条件控制基础

---

## 🔁 1. `for` 循环

### ✅ 用于：遍历列表、字符串、范围
```python
for i in range(5):
    print(i)  # 输出 0~4
```

### 常用结构：
- 遍历范围：`for i in range(start, end)`
- 遍历列表：`for item in list`
- 统计 / 累加：`sum += item`

---

## 🔄 2. `while` 循环

### ✅ 用于：**条件为真就一直执行**
```python
count = 0
while count < 3:
    print("还没到3")
    count += 1
```

### 常用结构：
- 输入验证（直到输入合法为止）
- 计数、反复操作直到满足条件
- 无限循环 + `break` 手动退出

---

## 🧯 3. 循环控制关键词

| 关键词 | 作用 |
|--------|------|
| `break` | 立即退出当前循环 |
| `continue` | 跳过当前这一次，进入下一次循环 |
| `pass` | 占位，不做任何操作（用于结构空白时） |

```python
for i in range(5):
    if i == 2:
        continue  # 跳过 2，不打印
    print(i)
```

---

## 🔎 4. 条件判断结构（if / elif / else）

```python
x = 5
if x == 5:
    print("等于5")
elif x > 5:
    print("大于5")
else:
    print("小于5")
```

### 常见用法：
- 多条件判断
- 嵌套在循环中一起用
- 判断输入是否合法 / 是否结束

---

## 🔢 5. 数值处理技巧

### 📦 常用操作：
- 拆数字：`while x > 0: digit = x % 10; x //= 10`
- 求最大值：`max(list)`
- 列表求和：`sum(list)`
- 统计出现次数：使用 `count()` 或字典

---

## 🧪 6. 字符串/列表小技能（用于 LeetCode）

| 目的 | 方法 |
|------|------|
| 转小写 | `s.lower()` |
| 判断数字 | `char.isdigit()` |
| 分割字符串 | `s.split()` |
| 去除前后空格 | `s.strip()` |
| 列表长度 | `len(arr)` |
| 找最大值 | `max(arr)` |
| 累加求和 | `sum(arr)` |

---

## 🧠 7. 项目/题目中用到的综合逻辑

### 举例：
- “你最多可以猜 3 次” → `while tries < 3:`
- “输入一个整数，直到合法为止” → `while True: try...except`
- “比较数组中每个数是否最大” → `for i in arr: if i + extra >= max_val:`

---

## ✅ 你在 Day 2 会重点使用：

| 语法 | 场景 |
|------|------|
| `for i in range(n)` | 累加 / 遍历 |
| `while condition` | 模拟流程 / 用户输入 |
| `if...elif...else` | 条件控制 |
| `break / continue` | 控制流程跳出或跳过 |
| 字符串/数字处理 | 与输入输出题结合使用 |
