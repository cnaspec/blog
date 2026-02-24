---
layout: post
author: Clodagh
---

In this task, we were expected to think about the requirements to create an online grocery shopping application.

## Assumptions Made

To convert this scenario into this data modeling framework, I had to made several assumptions.

First, I assumed there was no constraints on the fulfilment times or the number of workers required to fulfil an order (i.e. that there were always enough delivery drivers and vans to fulfil an order, and the distances between the deliveries did not need to be accounted for in the logistics, that the store is not closed on certain days or has blackout dates for delivery, no pickup orders will need to be rescheduled due to staff shortages, etc) in order to minimise the considerations. I further assumed that all customers who have an account have a phone number.

I also assumed that the choice of the subsitute items has been left to the discretion of the grocery picker and is not mandated by the system.

## User Stories

To quantify the importance of the stories, I use a 1 to 5 scale with 1 being the highest priority level and 5 being the lowest. All these user stories (with the exclusion of 5 due to the additional complexity) are small, as they are closely related to the initial requirements of the task.

1. Owner can add new items for sale
    -  Priority: 1
    - This is a necessary requirement that must be fulfilled.
2. Owner can specify the name, price, quantity available and the manufactuer and the manufacturer of the items for sale.
    - Priority: 2
    - This is an extremely important requirement to ensure the system works as intended.
    - This is linked to User Story 1 as it is related to the owner-centered experience of the system.
3. Customers can select the quantity of each item they wish to purchase.
    - Priority: 1
    - This is a necessary requirement that must be fulfilled.
4. Customers can select the method of fulfilment (pickup or delivery).
    - Priority: 2
    - This is an extremely important requirement to ensure the system works as intended.
5. Customers may wish to select which subsitute to recieve if a chosen item is out of stock.
    -  Priority: 5
    - This would be convenient for the customer but may be to the detriment of the owner. Whilst it would be nice to have it is no means necessary, which is why it has not been implemented in the diagrams.
6. Customers can select the date and time of order fulfilment.
    - Priority: 2
    - This is an extremely important requirement to ensure the system works as intended; however, it is notably more important for pick-up orders than delivery ones (unless the delivery orders include perishibles).
    - This is linked to User Story 4 as it is related to the method of order fulfilment and its logistics.


## Diagrams

### LucidChart Entity Relationship Diagram

![DEModel]({{ '/assets/images/\Lab 6_DE_Model.png' | relative_url }})

### RedGate Schema

![Schema]({{ '/assets/images/Lab_6_Schema.png' | relative_url }})

With regards to the above diagrams, I am not particularly satisfied with the representations above because I feel that I don't understand the concepts well enough to execute them competently. For example, when I was working on the Entity Relationship diagram (prior to working on the Schema) I kept thinking of validation and entities which would improve the systems function but was unclear on how these would actually be implemented in a database which prevented me from using them and this was frustrating.

I think the Entity Relationship diagram is an adequate representation of a very basic system that would satisfy the requirements. The issue is with the RedGate Schema, as the system would require a great deal of validation (such as ensuring customers don't select more quantity of a product than exists in inventory, or ensuring order fulfilment doesn't exceed the stores capacity to fill in terms of method, dates and times), and it is unclear to me how this might be implemented. To correct this, I need to do some further independent study on the topics to ensure I understand the fundementals properly.