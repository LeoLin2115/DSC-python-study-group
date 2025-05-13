Week5
CH.9 Tuple and Set
1. Tuple is element in parentheses tuple = (elements)
2. Tuple is immutable
3. if only one element in tuple you have to add common tuple = (element,)
4. Set is element in {} or set(elements)
5. set
    交集 data1.intersection(data2)
    聯集 data1.union(data2)
    差集 data1.difference(data2) data1 有 date2 沒有 in data1 but not in data2
6. set.add(element), set.remove(element)

CH. 10 Function 1
1. def func():
        statements
2. There is Indentation in python 
3. def func(*args, **kwargs):
    print(args, kwargs)
4. LEGB rule 「區域（Local, L）」、「封閉（Enclosing, E）」、「全域（Global, G）」以及「內建（Built-in, B）」
5. Python 的 Scope 只跟函數定義在什麼地方有關，跟它在哪裡被執行無關。
        language = "Python"

        def hi():
            print(language)

        def hey():
            language = "Ruby"
            hi()

        hey()
        print out Python

        language = "Python"

        def hey():
            def hi():
                print(language)

            language = "Ruby"
            hi()

        hey()
        print out Ruby 
6. global will call the first layer variable and nonlocal will call previous layer variable