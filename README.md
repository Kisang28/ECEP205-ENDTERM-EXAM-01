Exam Instructions AY2021-2022
------

1. Fork the given repository
2. Clone the your repository to your local machine
3. Create a development branch from the main branch. This is where you will make the changes
   1. At the Item class, complete the given operations of the following:
      1. Compute for the amount based on the price of the product multiply with quantity
      2. Compute amount when the quantity changes
      3. Compute amount when the quantity changes
   2 At the Order class, complete the given operations of the following:
      . Create a new item and append to the items list
      2. Remove an item from a given index
      3. Return the total quantity of an order (from items)
      4. Reutrn the overall total of an order (from items)
4. Commit the changes
5. Create a UnitTest Branch from the development branch, and do the following within the Unit Test Branch.
6. Create a unit test for the Order class that will test the following methods
   1 Create an item and check if the amount computed coincides with your expected computation
   2 Create an item, then use setProduct to change the product, then check if the amount computed coincides with your expected computation
   3 Create an item, then use setQuantity to change the quantity, then check if the amount computed coincides with your expected computation
7. Commit the changes and merge to the development branch
8. Go back to UnitTest Branch and do the following:
   1. Create a Unit Test for the Order class
   2. @BeforeAll, instantiate the order and add 5 items.
   3. Create a test method and add another 5 items to the order by using addItem and check if getTotalQuantity, and getGrandTotal methods returns what is expected
   4. Create a test method and remove 3 items from the order by using removeItem and check if getTotalQuantity, and getGrandTotal methods returns what is expected
9. Commit the changes and merge to the development branch
10. Push all branches to your repository
11. Create a pull request of your development branch

Note:
1. An order may include 1 or more items but an item is included in 1 order.
2. A Item includes only 1 product and a product is included in only 1 item.

Example.

Order No. #1

|Qty     |Product       |Price     |Amount|     |
--- | --- | --- | --- | --- |
|1 			|Item A 				|10.00 		 |10.00  |<-- Item 1|
|3 			|Item B				|20.00 		 |60.00  |<-- Item 2|
|2 			|Item C				|15.00 		 |30.00  |<-- Item 3|
|5 			|Item D				|30.00 		|150.00  |<-- Item 4|
|11  |<-- Total Quantity|           |250.00  |<-- Grand Total|  |

**Order**
-----

  - Items
    - Item # 1
      - Product
          - name : Item A
          - price : 10
      - quantity : 1
      - amount : 10
    - Item # 2
      - Product
         - name : Item B
         - price : 20
      - quantity : 3
      - amount : 60
    - Item # 3
       - Product
          - name : Item C
          - price : 15
       - quantity : 2
       - amount : 30
    - Item # 4
       - Product
          - name : Item D
          - price : 30
       - quantity : 5
       - amount : 150
    