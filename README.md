# kottans
https://github.com/yevhendidokha/kottans.git
def GetCreditCardVendor(n):
card = [int(d) for d in str(n)]
vendor = ''
a = []

		if(card[0]==4):
			vendor = "Visa" 
		elif ((card[0] == 3 and card[1] == 4) or (card[0] == 3 and card[1] == 7)):	
			vendor = "American Express"	
		elif ((card[0] == 5 and card[1] == 1) or (card[0] == 5 and card[1] == 2) or (card[0] == 5 and card[1] == 3) or (card[0] == 5 and card[1] == 4) or (card[0] == 5 and card[1] == 5)):
			vendor = "MasterCard" 
        elif( (a =[i for i in range(56,69)]: if a in card )	):	
			vendor = "Maestro"	
		elif( (a =[i for i in range(3528,3589)]: if a in card )	):	
			vendor = "JBC"	
		else 
		    vendor = "Unknown"
return vendor

print(GetCreditCardVendor(5533 1111 2222 3333))

GetCreditCardVendor()

def IsCreditCardNumberValid(n):
def d_of(n):
    return [int(d) for d in str(n)]

def luhn_checksum(card_number):
    ds = d_of(card_number)
    odd_ds = ds[-1::-2]
    even_ds = ds[-2::-2]
    total = sum(odd_ds)
    for d in even_ds:
        total += sum(ds_of(2 * dt))
    return total % 10

def is_luhn_valid(card_number):
    return luhn_checksum(card_number) == 0

return is_luhn_valid

IsCreditCardNumberValid(5533 1111 2222 3333)

IsCreditCardNumberValid()

from wheezy.core.luhn import luhn_sign
from wheezy.core.luhn import is_luhn_valid
 
GenerateNextCreditCardNumber = lambda n: '011d' % luhn_sign(n)

 
print(GenerateNextCreditCardNumber(5533 1111 2222 3333))
