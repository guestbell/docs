# Locations

GuestBell offer an option to create and assign specific locations to service items. This way, the guests can decide where the delivery will take place.

## Example usage

You offer a room service, but you also want to add an option to deliver these items directly to the pool area. To achieve this in GuestBell, you simply create 2 locations. "Room" and "Pool area". You then assign these locations directly to **service groups** or **service items**. Assigning to **service groups** can make things easier because the **services items** in said group will all use the configured locations.

## Overriding opening hours for locations

Consider this example. You serve continental breakfast in the restaurant. The restaurant have limited seating, therefore you [track the capacity](schedules.md) with your opening hours. Now you want the option to deliver directly to the room. You simply add the locations and now guests can choose. But there's a catch. In this setup, the orders that go to the room would still take up space in your restaurant.

To circumvent this issue, we have added an option to override the opening hours with each location. In this case, you would simply create a clone of the opening hours, but instead of using a time-span with capacity, you would simply un-tick the use capacity option and this will take care of the problem.

![Locations](https://static.guestbell.com/img/docs/locations/resource-locations.jpg)
