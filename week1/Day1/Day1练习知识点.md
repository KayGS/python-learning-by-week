**Day 2 Python LeetCode 做题知识点总结**

---

### 【一、LeetCode 题目总览】

- ܉ 转小写 (To Lower Case)
- 1108 转化 IP 地址 (Defanging an IP Address)
- 2114 找最多单词的句子 (Maximum Words in a Sentence)
- 1662 判断两个字符串数组是否相等 (Check If Two String Arrays are Equivalent)
- 1528 打乱字符串 (Shuffle String)
- 344 反转字符串 (Reverse String)

---

### 【二、字符串 vs 列表 基础区分】

| 概念 | 示例 | 类型 |
|--------|------|--------|
| 字符串 | "hello" | str |
| 列表 | ["h", "e", "l"] | list |

- 字符串无法直接修改内容，列表可以用索引直接设置值
- 如需要转换：`list(s)` 可以把字符串转为列表

---

### 【三、Python 常用字符串操作】

- `s.lower()` 把 s 全部转小写
- `s.upper()` 转大写
- `s.split()` 把字符串按空格分割成列表
- `" ".join(list)` 把列表重新联接成字符串
- `len(s)` 返回字符串/列表的长度

---

### 【四、for 和 while 循环】

#### 1. for 适合从列表/字符串中一个个取
```python
for i in range(len(s)):
    print(s[i])
```

#### 2. while 适合按照条件自动做多次
```python
left = 0
right = len(s) - 1
while left < right:
    s[left], s[right] = s[right], s[left]
    left += 1
    right -= 1
```

---

### 【五、反转字符串矩阵思路】

- 使用左右指针同时从两头向中间移动
- 使用 swap:
  ```python
  s[left], s[right] = s[right], s[left]
  ```
- 这种用途叫做 Python 的 “一行互换形式”

---

### 【六、小知识点】

- `==` 是用来判断是否相等
- `=` 是赋值
- `res = [""] * len(s)` 用于创建空格字符串列表
- `res[indices[i]] = s[i]` 表示把 s[i] 放到新的指定位置
- `a, b = b, a` 是 Python 中互换值的简单写法

