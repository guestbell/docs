?> This is an **Expert mode** feature. Make sure [it's enabled](overview.md?id=advanced-features) if you cannot find it in the dashboard.

# Packages

It's is common in hospitality to sell services via packages. You can for instance have **Breakfast included**, **Half-board**, **Full-board** and **All inclusive**. GuestBell supports this via **Packages**. You can find them in **Property -> Services -> Packages**.

You can create a package on this page by clicking the create button.

![tags](https://static.guestbell.com/img/docs/packages/create.png)

1. _Title_ - Name of the package that will also be presented to the guest
2. _Visible in self check-in_ - Based on your configuration, guests might be able to self-check-in to your property. In such case, you can decide if you want to let them indicate which packages are included in their stay. Otherwise your staff would need to do this in the check-in details page. Check this checkbox to allow guest to add this package when they check-in
3. _On by default_ - Check this to force this package for every newly checked in guest.

Once created, you can choose if **service groups** or **items** are included or excluded in a given packages. To do this, navigate to **group** or **item details page** and locate the **Packages section**.

?> **Tip** Service items and groups included in packages will be hidden by default for guests who are not checked-in to GuestBell.

## Publicly visible packages

Previously, we mentioned services included/excluded in packages will be hidden on your public page. The public page is used before the Guest is checked into GuestBell. This is because there's no way to determine which packages will the guests use once they check in.

There is however a way to overcome this, even for the public page. This information can be included in the check-in QRCode or URL. The most convenient way to do this is using **Deep links**.

1. Navigate to **Property -> Deep links**
2. Open the **Self check-in information** section
3. Under the **Check-in** sub-section, locate the **Packages** field
4. Here you can add the packages that you want to be included in this URL
5. Create different QRCodes or URLs based on your use case. For instance, if you have **Half board** and **Full Board** options, simply create 2 QRCodes and present it to your guests based on which option they use.
