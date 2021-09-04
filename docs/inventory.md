# Inventory

GuestBell comes with a powerful and easy to set-up inventory management system. Your inventory will also be automatically updated every time an order is placed/delivered.

## High level overview

Setting up inventory in GuestBell is straight forward. All you have to do is:

1. Enable inventory for your property
2. Create inventory items
3. Configure inventory consumption per service item
4. Restock inventory when necessary
5. Monitor consumption using logs

Now we will look at these steps in more details

## Enable inventory

Start by navigating to **Property -> Edit property**. Here you will find a section title "Inventory" that looks similar to the following image.

![inventory section](https://static.guestbell.com/img/docs/inventory/inventory-section.jpg)

### Enabled

Useful for temporarily enabling or disabling inventory tracking

### Validate new orders

- **Checked** - new orders will be rejected with an error if there is not enough inventory to fullfil them
- **Unchecked** - there is no orders validation. This way, the inventory quantities can become negative. It might be useful to choose this option if you want to track inventory changes solely for information purposes

### Service item out of stock behaviour

Changes how service items are displayed in the guest app when they are no longer available

- **Warning** - a warning will be displayed
- **Hidden** - service item is completely hidden

## Create inventory items

Navigate to **Property -> Inventory -> Items**. Then click the create button in the top right corner. Following modal will open.
![create inventory item](https://static.guestbell.com/img/docs/inventory/inventory-section.jpg)

### Title

Easily recognizable name of the inventory item such as "Pizza base, Dom Pérignon Vintage 2010 ..."

### Unit

Unit at which the item will be counted. E.g. "piece, liter, kg ..."

### Quantity

An initial quantity of the product

### Alert threshold

We will send you a "Low inventory warning" email once quantity dips bellows the number configured here. Leave blank to disable the email warning.

### Tags

You can assign a tag to the inventory item, this will make it easier to restock items later. Use tags such as "Beverages, Butchery, Food ..."

?> **Tip:** Granularity at which you track items is totally up to you. You can track "pizza base" or you can track "flour, yeast, water, salt, olive oil" separately. You can choose to only track some items (like expensive alcohol bottles) and not track more disposable items such as vegetables or fruit.

## Configure inventory consumption per service item

You will find a new section in your [service item](services.md#service-details) titled "Inventory consumption". Use the "Pick" button in the top right corner of this section to find the inventory items this service consumes.

Once you add the inventory items, you can use the consumption column of the table to configure consumption per unit ordered.
![inventory consumption section](https://static.guestbell.com/img/docs/inventory/inventory-consumption-section.jpg)

## Restock inventory when necessary

Navigate to **Property -> Inventory -> Items**. Then click the restock button in the top right corner. Following modal will open.
![restock modal](https://static.guestbell.com/img/docs/inventory/restock-modal.jpg)

### Add one by one

You can select which items to restock one by one

### Add by tags

You can select which items to restock by tags

### Comment

Type a comment which will be included with in the logs

### Table

Items you select will be displayed in this table. You can then change how much quantity will be added in the Quantity change column

### Change blocked quantity

There are limited situations when the blocked quantity becomes "out of sync" and yields negative or positive number even with no pending orders. This only happens if you change service item consumption while the order is pending. When this happens, you can fix it by directly changing the blocked quantity

## Monitor consumption using logs

Navigate to **Property -> Inventory -> Logs**. You will be presented with a table of all events that changes quantity of your inventory items. Part of the details will be a link to the employee who performed the change (restocking) or the order that used inventory. You will also see exact amount of change per item and comment (if present) so that you have full visibility into your inventory tracking
