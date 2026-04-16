from abc import ABC, abstractmethod

class Payment(ABC):
    @abstractmethod
    def __init__(self, x):
        pass

class CardBill(Payment):
    def __init__(self, x):
        print("CardBill:", x)

class BankBill(Payment):
    def __init__(self, x):
        print("BankBill:", x)

# Example usage
c = CardBill("Paid with card")
b = BankBill("Paid via bank")
