# Exam
import numpy as np
import pandas as pd

Class Shopping:
       def _init_(self,groceries{}):
         basket = {eggs:20, rice:25, flour:30, sugar : 40}
         price = {eggs:1,rice:30,flour:1.25,sugar:.99}
        discount={}
        shoplist = []
        add = input("Want to add something to your shopping list? Y or N'")
    while.add.lower() == "y":
    item = input("Enter your item to the list:")
    shoplist.append(item)
    add = input("Want to add to your shopping list? Y or N")
    print ()
    shoplist.sort()
    for listitem in shoplist:
        print(listitem)
shoplist = []
add = input("Want to add something to your shopping list? Y or N'")
while add.lower() == "y":
    item = input("Enter your item to the list:")
shoplist.append(item)
add = input("Want to add to your shopping list? Y or N")
print ()
shoplist.sort()
for listitem in shoplist:
    print(listitem)
Items_discount = {"eggs":20, "rice":32,"Flour":5}
items_price = {"eggs":5,"Rice":55,"Flour":60}
def returning_prices(basket):
    total_prices_basket = []
    price_of_each_item = []
    for i in basket:
        if i in items_price.keys():
            price_of_item = items_price[i]
            discount = Items_discount[i]
            price_after_disc = price_of_item*(1-discount/100)
            price_of_each_item.append(price_after_disc)
        else:
            return 0;
        total_prices_basket.append(sum(price_of_each_item))
        return total_prices_basket
print(returning_prices(['eggs','rice','Flour']))
Items_discount = {'eggs':20,'rice':32,'flour':5}
items_price = {'eggs':5,'rice':55,'flour':60}
def returning_prices(basket):
    total_prices_basket=[]
    
    for j in basket:
        price_of_each_item=[]
        for i in j.keys():
            
            if i in items_price.keys():
                price_of_item = items_price[i]
                discount = Items_discount[i]
                price_after_disc = price_of_item*(1-discount/100)
                price_of_each_item.append(price_after_disc*j[i])
                
            else:
                break;
        total_prices_basket.append(sum(price_of_each_item))
        total_prices_basket.sort(key=None, reverse=True)
    return total_prices_basket
basket=[{'eggs':5,'rice':2},{'flour':5,'rice':2},]
print(returning_prices(basket))
