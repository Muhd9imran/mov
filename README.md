class Acount:
  def __init__(self,bal,acc):
    self.balance=bal
    self.account_no=acc

  def debit(self,amount):
    self.balance -= amount
    print("Rs",amount,"was debited")
    print("Total balance=",self.get_balance())  

  def credit(self,amount):
    self.balance += amount
    print("Rs",amount,"was credited")
    print("Total balance=",self.get_balance())
  def get_balance(self):
    return self.balance  

acc1=Acount(222220,12345)

acc1.credit(200000)
acc1.debit(500)
maaz=Acount(0,124)
maaz.credit(100000)
