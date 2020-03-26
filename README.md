# Exam

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

  #price per quantity
items_price = {"eggs":5,"rice":30,"flour":50}
#discount is in percentage
Items_discount={"eggs":20,"rice":10,"flour":10}

class shopping_basket:
    def __init__(self,basket):
        self.__basket=basket
    def returning_prices(self):
        total_prices_basket=[]
       
        for j in self.__basket:
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
basket=[{'eggs':5,'rice':2},{'flour':5,'rice':2}]
object = shopping_basket(basket)
j=object.returning_prices()
print(j)

