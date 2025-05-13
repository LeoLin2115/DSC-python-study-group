Week5
CH.11 Function 2
1. Expression have result (return value) but statement not
2. Lambda experssion $lambda parameters: expression
3. map, filter with lambda 
    numbers = [1, 2, 3, 4, 5]
    double_numbers = map(lambda x: x * 2, numbers)
    print(list(double_numbers))

    numbers = [1, 2, 3, 4, 5]
    even_numbers = filter(lambda x: x % 2 == 0, numbers)
    print(list(even_numbers))
4. Closure: When one variable is in multiple scopes, then python create cell object point to vairalbe
5. Decorator: 
6. 語法糖
7. Genarator: yield
    def even_numbers(n):
    i = 1
    while i <= n:
        if i % 2 == 0:
            yield i  # <- 在這裡
        i += 1
    nums = even_numbers(10)
    [n for n in nums]