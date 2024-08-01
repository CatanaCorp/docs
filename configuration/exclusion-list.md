---
description: Ignore TODOs from files of your choice
---

# Exclusion list

<div align="center" data-full-width="true">

<figure><img src="../.gitbook/assets/Exclusion list.png" alt="" width="563"><figcaption></figcaption></figure>

</div>

Catana can automatically ignore upcoming TODOs based on their file path. Any existing or upcoming TODOs matching the paths you have configured will be [ignored](../core-concepts/ignored-todos.md).

{% hint style="info" %}
The autocompletion field will help you configure the paths you want to ignore.\
\
Pro tip: If you need to fine-tune the paths, the field accepts any valid shell glob pattern.
{% endhint %}

***

Modifying the exclusion list will prompt you to decide whether you'd like to ignore existing TODOs now matching the list.

<figure><img src="../.gitbook/assets/Exclusion list confirmation.png" alt="" width="375"><figcaption></figcaption></figure>

When a new TODO is added to your codebase in a path that matches the exclusion list, **Catana will not**:

1. Run any [validation](../core-concepts/validation.md).
2. Open a ticket in your issue tracker (if the repository has opted in for [this feature](open-github-issues.md)).
