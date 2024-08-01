---
description: Ignore TODOs from files of your choice
---

# Exclusion list

<div align="center" data-full-width="true">

<figure><img src="../.gitbook/assets/Exclusion list.png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Catana can automatically ignore a TODO based on its file path (you can also ignore TODOs manually). Any existing or upcoming TODOs matching the paths you have configured will be "[soft ignored](exclusion-list.md#ignored-todo)".

{% hint style="info" %}
The autocompletion field will help you configure the paths you want to ignore.\
\
Pro tip: If you need to fine-tune the paths, the field accepts any valid shell glob pattern.
{% endhint %}

***

Modifying the exclusion list will prompt you to decide whether you'd like to ignore existing TODOs now matching the list.

<figure><img src="../.gitbook/assets/Exclusion list confirmation.png" alt="" width="375"><figcaption></figcaption></figure>

## Ignored TODO

Catana will not fully ignore a TODO added to your codebase. A TODO matching the exclusion list will still be processed and recorded; however, Catana will treat these TODOs differently:

* Ignored TODOs will not be [validated](../core-concepts/validation.md).
* Catana will not open a ticket in your issue tracker.
* No reminders will be sent.
* Ignored TODOs will not be counted in the stats shown on your dashboard.
