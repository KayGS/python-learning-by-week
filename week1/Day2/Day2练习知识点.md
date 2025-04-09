## ✅ 1365. How Many Numbers Are Smaller Than the Current Number

**目标：** 对每个元素，计算有多少个数小于它。

**知识点：**
- 双重 `for` 循环嵌套
- 计数器变量 `count`
- `range(len(nums))` 遍历列表索引
- 列表追加 `.append()`

---

## ✅ 383. Ransom Note

**目标：** 判断 ransomNote 是否可以由 magazine 组成。

**知识点：**
- 字符频率统计
- `.remove()` 不推荐频繁用于字符串
- 使用 `collections.Counter` 进行计数更高效
- 哈希表思想：用字典判断字符是否足够

---

## ✅ 876. Middle of the Linked List

**目标：** 找出链表的中间节点。

**知识点：**
- 链表结构基础：`ListNode`
- 用列表暂存链表中的节点 `target = []`
- 利用 `len(target)//2` 找中间位置
- 遍历链表：`while cur: cur = cur.next`

---

## ✅ 1431. Kids With the Greatest Number of Candies

**目标：** 判断每个小朋友加上额外糖果后是否能成为最多的。

**知识点：**
- 使用 `max()` 函数找最大值
- 遍历元素 vs 遍历索引：`for c in candies`
- 每个元素与最大值对比，追加布尔值结果

---

## ✅ 2535. Difference Between Element Sum and Digit Sum

**目标：** 所有元素之和 与 所有数字位之和 的差。

**知识点：**
- 拆位处理：`for ch in str(num)`
- 数字转字符串：`str()`，再转回整数：`int()`
- 累加平方和的函数封装
- `sum(nums)` 和 `digit_sum` 的比较

---

## ✅ 58. Length of Last Word

**目标：** 返回字符串中最后一个单词的长度。

**知识点：**
- 字符串预处理：`strip()`, `split()`
- `split()` 默认按空格切割
- `[-1]` 访问列表最后一项
- `len(...)` 获取长度

---

## ✅ 2299. Strong Password Checker II

**目标：** 判断一个字符串是否是强密码。

**知识点：**
- 多条件判断：`if / elif`
- 字符串判断函数：`islower()`, `isupper()`, `isdigit()`, `char in specials`
- 连续字符判断：`password[i] == password[i - 1]`
- 状态记录布尔变量：`has_lower = False`
- `return` 的位置对控制逻辑的影响

---

## ✅ 额外补充的语法技巧：

| 技能点 | 用法 / 示例 |
|--------|-------------|
| 多变量同时赋值 | `a = b = c = False` |
| 条件组合 | `return A and B and C` |
| 函数定义与调用 | `def get_sum(n): ...` → `get_sum(19)` |
| `for i in range(...)` vs `for char in s` | 是否需要索引决定用法 |
| 提前终止判断 | `if 条件: return False` |
| 字符串是不可变对象 | `.remove()` 不适用于字符串 |
"""

