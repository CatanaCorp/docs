---
description: Create multiple TODOs referencing the same issue.
---

# Overview

It is quite common to have multiple TODOs in a project referencing the same ticket. This allows developers to highlight related chunks of code and create a sort of task list, with each TODO acting as an anchor.

Catana includes a feature to improve this workflow and help resolve related TODOs.

<figure><img src="../.gitbook/assets/Group overview.png" alt="" width="563"><figcaption></figcaption></figure>

### Reference

Any TODO with a title that includes the keyword `Ref #123` (Where 123 is the number of a **opened** issue in your GitHub tracker) would be grouped together with other TODOs with the same reference.

<figure><img src="../.gitbook/assets/Group code example.png" alt="" width="375"><figcaption></figcaption></figure>

The first time a ticket is referenced in a TODO, Catana creates a comment on the referenced issue, indicating the line and file that require attention.\
As more TODOs referencing the same ticket are added, Catana updates the previously created comment and the task list.

\
When a TODO that was part of a group is removed from the codebase, Catana reflects this and updates the task list.

<figure><img src="../.gitbook/assets/TODO removed from group.png" alt="" width="563"><figcaption></figcaption></figure>

Finally, when all TODOs have been removed, Catana considers the ticket solved and will inform your team by commenting on the ticket.

<figure><img src="../.gitbook/assets/All todos removed from group.png" alt="" width="375"><figcaption></figcaption></figure>

{% hint style="info" %}
Any time a TODO that is part of a group changes location (line or file), Catana reflects the change.

The task list will always remain up to date, eliminating the need to search through the git history.
{% endhint %}

### Dashboard

When viewing a TODO item on the Catana dashboard, a list of related TODOs is displayed.

<figure><img src="../.gitbook/assets/TODO group dashboard.png" alt="" width="563"><figcaption></figcaption></figure>
