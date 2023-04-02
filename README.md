# Linked_list

Here I tried to figure out how linked list works. First time i met this topic on hackerrank 30 Days of Code, where different issues were presented. I couldn't understand how does it work and I even take a bit long break for a month. After that I came back to solve it and thats what i have.  

    class Node:
        def __init__(self,data):
            self.data = data
            self.next = None 
    class Solution: 
        def display(self, head):
            current = head
            while current:
                print(current.data,end=' ')
                current = current.next

        def insert(self, head, data): 
            newNode = Node(data)
            if head == None:
                head = newNode
            else:
                current = head
                while current.next:
                    current = current.next
                current.next = newNode
            return head

    mylist = Solution()
    T=int(input())
    head=None
    for i in range(T):
        data=int(input())
        head=mylist.insert(head,data)    
    mylist.display(head)
    
This code create linked list.
  
I got a lot of motivation after watching Winderton (https://www.youtube.com/@wndtn) videos. I discovered a large area of study and have a lot of interest to study everything connected with modern programming.
