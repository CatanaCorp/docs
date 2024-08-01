# Ignored TODOs

You have the option to ignore an already recorded TODO or [create an exclusion list](../configuration/exclusion-list.md) to ignore upcoming and existing TODOs based on their file path.\
Ignoring and destroying a TODO are different actions, and this page outlines what ignoring a TODO actually does.

Catana treats ignored TODOs differently in the following ways:

* Todo item records will be **visible on a separate page** on your dashboard.
* Ignored TODOs will **not be counted in the stats** shown on your dashboard.
* Ignored TODOs have no assignee.
* No reminders will be sent.
* You can't create a ticket in your issue tracker.

<figure><img src="../.gitbook/assets/Ignored TODOs.png" alt="" width="563"><figcaption><p>The tab displaying all ignored Todo items.</p></figcaption></figure>



As your project evolves, Catana will continue monitoring ignored TODOs and update records accordingly (e.g. the TODO moves to a different line or file).

{% hint style="info" %}
**A note on this design choice:**

\
Catana simply reflects and highlights the developer annotations from your codebase, and as such, will only destroy a record if the corresponding TODO comment in your project is removed.

There are no other ways to destroy a TODO from Catana; this is by design.
{% endhint %}

### Manually ignore a Todo item

To ignore an already existing Todo item, first find it on your Catana dashboard, then click to view all of its details, and finally click on the "Ignore this TODO" button.

### Ignore existing and upcoming Todo items based on their file path

See the [exclusion list documentation page](../configuration/exclusion-list.md).





