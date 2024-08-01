# Rules

<figure><img src="../.gitbook/assets/Catana Rule.png" alt="" width="563"><figcaption></figcaption></figure>

\
When a TODO remains unresolved after a given period, Catana will perform an action of your choice, such as sending an email reminder to its assignee.

### Adding rules

To create a rule, click on the "Add a rule" button. Each rule you add requires two inputs:

1. The number of days after a TODO is introduced before the rule should kick in.
2. The action to perform.

{% hint style="info" %}
There is only one action available as of today, which is "Remind the TODO author."

Other actions, such as "Remove the TODO from the codebase," will be implemented in the future.
{% endhint %}

For instance, you can configure one reminder two weeks after a TODO is introduced, a second reminder two more weeks later, and finally remove the TODO from the codebase if it has not been resolved after two months.

#### :warning: Note

Adding a new rule will apply to both upcoming and existing TODOs.

For example, if you add a new rule to remind the author two weeks after a TODO is introduced, the rule will take effect for any existing TODOs that were added two weeks ago or earlier.

\
