
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

