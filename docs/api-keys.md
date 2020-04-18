# Api keys

You can find api keys in **Property -> Developers -> Api keys**

Usually, it is enough to work with a service using the user interface just like our GuestBell dashboard. However, sometimes, you need a machine or a service to interface with the system. This can be a check-in machine, room-tablet or a front desk terminal. For this reason, GuestBell has an [API](https://api.guestbell.com) - [Application programming interface](https://en.wikipedia.org/wiki/Application_programming_interface). Using this tool, you can work with any aspect of GuestBell programmatically.

In order to secure this communication, you need to send a special key as part of every request sent to the system using the [HTTPS](https://en.wikipedia.org/wiki/HTTPS). This key is commonly referred to as an [Api key](https://en.wikipedia.org/wiki/Application_programming_interface_key).

Api key should be sent as part of Authorization header in the following form:
apiKey {yourApiKey}

You can create these keys using the modal shown on the image bellow.

![Add api key modal](https://static.guestbell.com/img/docs/api-keys/modal.jpg)

A _name_ can be created for an api key to help determined where it is used. You also need to assign a [Permission group](permissions.md) to the api key to limit what this connection can be used for. This works exactly the same as permissions for [employees](staff.md).

?> **Tip:** You can add expiration date to the api key. This is useful when you are working with 3rd parties.

Finally, you can access **Api Keys Details Page** by clicking the **DETAILS** button in the api keys table, you can reset an api key here, or edit it's properties.

![Api key table](https://static.guestbell.com/img/docs/api-keys/table.jpg)

?> **Tip:** Make it possible to easily change this key in your implementations via config files. You need to be ready to change it immediately in case your api key is compromised.
