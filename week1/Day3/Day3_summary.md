# 📘 Day 3 知识点讲解：列表操作与内置函数

## 🔢 一、列表（List）基本操作

### 1. 创建列表
```python
nums = [1, 2, 3, 4]
words = ["apple", "banana"]
```

### 2. 常用增删改查操作

| 操作       | 方法                           | 示例                      |
|------------|--------------------------------|---------------------------|
| 添加元素   | `list.append(x)`               | `nums.append(5)`         |
| 插入元素   | `list.insert(index, value)`    | `nums.insert(1, 10)`     |
| 删除元素   | `list.remove(value)`           | `nums.remove(3)`         |
| 弹出末尾   | `list.pop()` / `list.pop(i)`   | `nums.pop()`             |
| 修改元素   | 直接赋值                        | `nums[2] = 99`           |
| 查找索引   | `list.index(x)`                | `words.index("apple")`   |

---

## ✂️ 二、切片（Slicing）

切片语法：`list[start:end:step]`

```python
a = [1, 2, 3, 4, 5]
print(a[1:4])      # [2, 3, 4]
print(a[::-1])     # 倒序 [5, 4, 3, 2, 1]
print(a[:3])       # 从头到 index 2
```

---

## 🧰 三、内置函数 + 列表函数

| 函数         | 功能                   | 示例                |
|--------------|------------------------|---------------------|
| `len(lst)`   | 获取元素个数           | `len([1,2,3])` → 3  |
| `sum(lst)`   | 求和                   | `sum([1,2,3])` → 6  |
| `max(lst)`   | 最大值                 | `max([1,5,2])` → 5  |
| `min(lst)`   | 最小值                 | `min([1,5,2])` → 1  |
| `sorted(lst)`| 返回排序后新列表       | `sorted([3,1,2])`   |
| `in`         | 判断元素是否存在       | `3 in [1,2,3]` → True |

---

## 🔁 四、列表推导式（List Comprehension）

### ✅ 简洁写法（等价于 for 循环）

```python
# 传统写法
res = []
for x in nums:
    if x > 0:
        res.append(x)

# 推导式
res = [x for x in nums if x > 0]
```

适合过滤、转换、生成新列表。

---

## 🔄 五、字符串与列表转换

### 字符串转列表（拆分成字符）：
```python
s = "hello"
chars = list(s)   # ['h', 'e', 'l', 'l', 'o']
```

### 字符串分词（按空格切）：
```python
sentence = "I love Python"
words = sentence.split()  # ['I', 'love', 'Python']
```

### 列表转字符串（拼接）：
```python
chars = ['h', 'i']
s = "".join(chars)        # "hi"
```

---

## 🔎 六、枚举 + 条件 + 索引访问

使用 `enumerate()` 同时获取索引和值：
```python
for i, val in enumerate([10, 20, 30]):
    print(i, val)
```

使用条件判断：
```python
if len(nums) > 0 and nums[0] > 10:
    ...
```

---

## ✅ Day 3 最常见题型示例

| 类型             | 常见题目举例                        |
|------------------|-------------------------------------|
| 构造目标列表     | 1389. 按顺序创建目标数组             |
| 异或处理数组     | 1720. 解码异或数组                   |
| 差值处理         | 2574. 左右元素和的差值               |
| 字符操作         | 1108. IP 地址无效化、2810 整理字符串  |
| 列表推导统计     | 1773. 统计满足条件的项目             |

---

📌 看完这些，如果你已经理解或希望动手试试，我可以马上带你刷一题，例如：

> 🔹【1389. 按既定顺序创建目标数组】正好用到了 `insert()`！

需要我现在带你从这道题开始动手练吗？😄
