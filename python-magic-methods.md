##### __len__

You can do `len(obj)` after you define __len__() method inside the obj class
example:
~~~ python
class Stack:
    def __init__(self):
        self._stack = []

    def __len__(self):
        return len(self._stack)

    def __str__(self):
        return str(self._stack)

    def push(self, item):
        self._stack.append(item)
  
obj = Stack()
obj.push(1)
obj.push(3)
obj.push(4)
print(len(obj))
print(obj)
~~~
Outputs:

      3
      [1, 3, 4]
