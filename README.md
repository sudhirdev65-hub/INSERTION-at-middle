class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
n1=Node("oorum blood")
n2=Node("thee ithu Thalapathy")
n3=Node("TVK flag anthem")
n4=Node("unga vijay")
n1.next=n2
n2.next=n3
n3.next=n4
head=n1
def display(head):
     temp=head
     while temp is not None:
         print(temp.data,end="->")
         temp=temp.next
     print("None")
print("Original Linked List")
display(head)
print("Insertion in the middle")
new_node=Node(" Naa ready tha varava")
temp=head
while temp.data!=" Thee ithu Thalapathy":
    temp=temp.next
new_node.next=temp.next
temp.next=new_node
display(head)