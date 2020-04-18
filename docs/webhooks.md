# Webhooks

You can find webhooks in **Property -> Developers -> Webhooks**

Sometimes, your applications, machines connected to the system or 3rd parties needs to react to events taking place inside the GuestBell system. This kind of [Api integration](api-integrations.md) is usually achieved by a technology called [Webhook](https://en.wikipedia.org/wiki/Webhook). It can be easily explained in a few short steps.

1. You create a publicly visible [API endpoint](https://en.wikipedia.org/wiki/Application_programming_interface)
2. You create a webhook (in application that supports webhooks) that fires a request to said endpoint every time a configured event occurs.
3. You accept and **verify** the origin of the call.

The verification of the webhook is usually done by signing a webhook data using a special function. This function takes a **Signing secret** and the data as arguments and outputs a **Signature**.

When you create a webhook in GuestBell we generate a **Signing secret** and use it to sign all requests fired to this webhook. You then generate the signature on your side using the **Signing secret** and compare the 2 signatures. If they match, you have a guarantee the request came from GuestBell.

In GuestBell, you can create a webhook using the modal shown bellow.

![Add webhook modal](https://static.guestbell.com/img/docs/webhooks/webhook-modal.jpg)

**Webhook details page** is where you can further configure you webhook. You will find it by pressing the **DETAILS** button in the webhooks table.

![Webhooks table](https://static.guestbell.com/img/docs/webhooks/webhook-table.jpg)

?> **Tip** You can temporarily disable webhook from firing using the **Status** dropdown on the **Webhook details page**.

![Webhook details](https://static.guestbell.com/img/docs/webhooks/webhook-details.jpg)
