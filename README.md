from idlelib.configdialog import changes

print("==============================================")
print("                 FM GROCERY                   ")
print("==============================================\n")
print("[PRODUCTS]                    DATE: 12/3/24")
print("\n-----------------CANNED-----------------")
print("[1]Corned Beef (150g)            - P70.12")
print("[2]555 Tuna (155g)               - P45.23")
print("[3]Century Tuna (155)            - P75.11")

print("\n----------------PASTRIES----------------")
print("[4]Gardenia Classic WB (600g)    - P90.42")
print("[5]Gardenia High Fiber WB (400g) - P93.76")
print("[6]SariMonde Tasty Bread (450g)  - P91.12")

print("\n-----------------SNACKS-----------------")
print("[7]Nagaraya (160g)               - P49.42")
print("[8]Potato Fries Ketchup (35g)    - P65.59")
print("[9]Oishi Pillows Choco (38g)     - P14.21")

print("\n-----------------ALCOHOL----------------")
print("[10]Alfonso Light (1L)           - P290.42")
print("[11]Alfonso Platinum (1L)        - P380.53")
print("[12]RedHorse (100ml)             - P90.21")
print("\n==============================================\n")

num = int(input("Product Number: "))

if num == 1:
    product = "Corned Beef (150g)"
    price = 70.12

elif num == 2:
    product = "555 Tuna (155g)"
    price = 45.23

elif num == 3:
    product = "Century Tuna (155g)"
    price = 75.11

elif num == 4:
    product = "Gardenia Classic WB (600g)"
    price = 90.42

elif num == 5:
    product = "Gardenia High Fiber WB (400g)"
    price = 93.76

elif num == 6:
    product = "SariMonde Tasty Bread (450g)"
    price = 91.12

elif num == 7:
    product = "Nagaraya (160g)"
    price = 49.42

elif num == 8:
    product = "Potato Fries Ketchup (35g)"
    price = 65.59

elif num == 9:
    product = "Oishi Pillows Choco (38g)"
    price = 14.21

elif num == 10:
    product = "Alfonso Light (1L)"
    price = 290.42

elif num == 11:
    product = "Alfonso Platinum (1L)"
    price = 380.53

elif num == 12:
    product = "RedHorse (100ml)"
    price = 90.21
else:
    print("Invalid Input.")
    exit()

q = int(input("Quantity: "))

if q <= 0:
    print("Invalid Quantity.")
    exit()

subt = price * q

if subt >= 1500:
    dis = 0.25
elif subt >= 1000:
    dis = 0.20
elif subt >= 500:
    dis = 0.10
else:
    dis = 0

disc = subt * dis
dis_amt = subt - disc
tx = dis_amt * 0.12
ftot = dis_amt + tx

print("\n==============================================")
print("                   RECEIPT                   ")
print("==============================================\n")
print(f"Product Number : {num}")
print(f"Price          : P{price}")
print(f"Quantity       : {q:.0f}")
print("==============================================")
print(f"Subtotal       : P{subt:.2f}")
print(f"Discount       : P{disc:.2f}")
print(f"Taxe           : P{tx:.2f}")
print("==============================================")
print(f"Total          : P{ftot:.2f}")
print("==============================================")

paym = float(input("Enter your Payment: P"))

if paym >= ftot:
    change = paym - ftot
    print(f"Payment : P{paym:.2f}")
    print(f"Change  : P{change:.2f}")
else:
    balance = ftot - paym
    print(f"Insufficient Balance.")
    print(f"Balance : {balance:.2f}")
print("\n----------THANKYOU FOR YOUR PURCHASE----------")
