# Rules

<figure><img src="../.gitbook/assets/Catana Rule.png" alt="" width="563"><figcaption></figcaption></figure>

\
When a TODO remains unresolved after a given period, Catana will perform an action of your choice, such as sending an email reminder to its assignee.

### Adding rules

To create a rule, click on the "Add a rule" button. Each rule you add requires two inputs:

1. The number of days after a TODO is introduced before the rule should kick in.
2. The action to perform.

{% hint style="info" %}
The number of days to wait will start at a different time depending on whether a TODO has a [trigger](../triggers/overview.md):

* For TODO items without a trigger, the timer starts at the time the TODO is introduced.
* For TODO items with a trigger, the timer starts when the TODO expires. If it has not yet expired, Catana will not perform any rules.
{% endhint %}

For instance, you can configure an email reminder two weeks after a TODO is introduced, a second reminder two weeks later, make the TODO more visible to the team by opening an issue after a month, and finally remove the TODO from the codebase if it has not been resolved after two months.

#### :warning: Note

Adding a new rule will apply only to upcoming TODOs.

For example, if you add a new rule to remind the author two weeks after a TODO is introduced, the rule will **not take effect** for existing TODOs, even if they were added two weeks ago or earlier.

\
