?> This is an **Expert mode** feature. Make sure [it's enabled](overview.md?id=advanced-features) if you cannot find it in the dashboard.

# Api Integrations

It is common for modern applications, machines and services to communicate with each other. This process is commonly called **Integration**. There are 2 kinds of communication. We will call these **IN-Integration** and **OUT-Integration**.

**IN-Integration** occurs when one service sends information to another service.

Example: Coffee is ordered in a IOT coffee machine. This coffee machine sends information to GuestBell regarding the order for the coffee. That means the message comes **IN**to the system.

We need to secure this communication and this is where [**Api keys**](api-keys.md) are used.

**OUT-Integration** deals with the problem of reacting to an event taking place.

Example: You have a service that prints WiFi password every time a guest is checked-in. In this case, GuestBell needs to contact the printer to start work. Therefore the message goes **OUT** of the system.

This kind of communication is achieved using [Web-hooks](webhooks.md).
