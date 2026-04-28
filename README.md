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