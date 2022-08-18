# match-chetnost
Функция для проверки четности числа
# ваша функция, её минус в том что она возвращает остаток
def values(value): return value % 2

# моя функция показывает само число и отвечает чётное оно или нет

def math(x):
    if x % 2 == 0:
        return f'Число {x} четное'
    else:
        return f'Число {x} не четное'

# 2 задание я вас не понял что вы хотите

# 3 задание

import random as r
nums = [1,2,3,4,5,6,11,7,8,9,10,13, 12,15,14]


def math(nums):
   if len(nums) <= 1:
       return nums
   else:
       q = r.choice(nums)
   l_nums = [n for n in nums if n < q]
 
   e_nums = [q] * nums.count(q)
   b_nums = [n for n in nums if n > q]
   return math(l_nums) + e_nums + math(b_nums)
  
print(math(nums))

