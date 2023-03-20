# Simple-Queue Data Sturcture

class Queue:
    def __init__(self) -> None:
        self.queue = []
    
    def enqueue(self, item):
        self.queue.append(item)
        
    def dequeue(self):
        if len(self.queue) < 1:
            return None 
        return self.queue.pop() 
    def display(self):
        print(self.queue) 
        
    def size(self):
        return len(self.queue)
    
obj = Queue()
obj.enqueue("khan")
obj.enqueue("waqar")
obj.enqueue("uzair")
obj.enqueue("ibrar")

obj.enqueue("lala")
obj.dequeue()
obj.dequeue()
obj.dequeue()
obj.dequeue()


obj.display()
