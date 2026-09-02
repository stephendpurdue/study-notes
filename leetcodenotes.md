
#### 412. Fizz Buzz

We created an empty list, then created a for i in range of 1, and n+1 so it increments. We then used if, elif, else to check if 'i' was divisible by 3 and 5, 3, and 5. The answer was then converted to a string and appended to the original list.
```
class Solution:
    def fizzBuzz(self, n: int) -> List[str]:
        ans = []

        for i in range(1, n+1):
            if i % 3 == 0 and i % 5 == 0:
                ans.append("FizzBuzz")
            elif i % 3 == 0:
                ans.append("Fizz")
            elif i % 5 == 0:
                ans.append("Buzz")
            else:
                ans.append(str(i))

        return ans

```
#### 458. Max Consecutive Ones

We set two values as 0 (res and cnt), then looped through the array, incremented the count if it was a consecutive, if not, the count was set to zero. res was set to the max of (cnt and res) to avoid rechecking the array.

```
class Solution:
    def findMaxConsecutiveOnes(self, nums: List[int]) -> int:
        res = cnt = 0

        for num in nums:
            cnt = cnt + 1 if num else 0
            res = max(cnt, res)
        return res
```

#### 217. Contains Duplicate

We created a HashMap, and then looped through the nums array, if the number was already in the map, we returned true, else, we added it to the HashMap. If it wasn't a duplicate, we returned false.

This is because each number was assigned a key value pair, upon looping through the nums array, if it was a duplicate, the value was increased by one.

```
class Solution:
    def containsDuplicate(self, nums: List[int]) -> bool:
        seen = set()

        for i in nums:
            if i in seen:
                return True
            else:
                seen.add(i)
        return False
```
