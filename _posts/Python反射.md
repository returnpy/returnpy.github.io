# Python反射

- 反射就是可以通过字符串的形式操作对象的属性

  ```python
  class Person:
      def __init__(self, name, age)
      	self.name = name
          self.age = age
          
  p = Person("Nicky", 18)
  
  if hasattr(p, "money"):
      print("哥们家里有钱")
  
  ```

  - getattr 获取对象的属性

  - hasattr 判断对象是否含有属性

  - setattr 给对象设置属性

  - delattr 删除对象的属性