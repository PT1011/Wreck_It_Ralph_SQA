# Wreck_It_Ralph_SQA
SQA Final Project - Jack and Parth

## Bug ID: BUG-01
### Bug Name: Test Max Health Enforced
#### Category: Boundary Failure
#### Location: shop.py
#### How to Trigger: Have health above 70, Use the health potion, observe the bug as your heath is above 100
#### Impact: The user could use potions over and over again until they have a ridiculous amount of health, in pvp this would cause an unfair advantage, in pve this could cause progression through the game that was not expected by the developers
#### Severity: High
#### Test File: from shop import Item, Player

## Bug ID: BUG-02
### Bug Name: Test Add Negative Quantity of Item
#### Category: Invalid Input 
#### Location: shop.py
#### How to Trigger: Add a number that is negative to the stock list 
#### Impact: If the stock is negative the player is unable to buy some items that they may have be able to otherwise 
#### Severity: High 
#### Test File: from shop import Item, Player

## Bug ID: BUG-03
### Bug Name: Test Buying Multiple Items 
#### Category: Silent 
#### Location: shop.py 
#### How to Trigger: Try to buy mupltiple of the same item, observe the bug 
#### Impact: 

def test_buying_multiple_items():
    """
    Expected: They shouldn't be the same object
    Actual: They are the same because of they way the code appends the objects as references to the memory
    Category: Silent
    Severity: Medium
    """