# Regular and expiring TODOs

{% hint style="info" %}
Catana can process and record all TODOs regardless on the syntax used. It also introduces a new type of TODO that can **expire at the time or condition of your choice**.
{% endhint %}

### <mark style="color:blue;">Regular TODOs</mark>

Catana processes all changes occurring on the release branch of enrolled repositories in real time. Any annotations using the **conventional keywords in all uppercase letters** (TODO, FIXME, BUG, XXX, NOTE) will be recorded.



<figure><img src="../.gitbook/assets/record-todos.png" alt="" width="563"><figcaption><p><strong>Examples of annotations Catana will record.</strong></p></figcaption></figure>

{% hint style="info" %}
Adding a semi-column ":" after the TODO declaration is supported but optional.
{% endhint %}

**The content that comes after the annotation keyword is treated as the description**. Adding a description is fundamental to helping your team members and future you understand why a TODO was added.

<figure><img src="../.gitbook/assets/todo-title.png" alt="" width="563"><figcaption><p><strong>The TODO description is reflected on the Catana dashboard.</strong></p></figcaption></figure>

\
Catana will automatically assign authors during the initial TODO recording. Authorship is determined based on the git commit. Authors will be assigned to their TODOs regardless if they ever signed in to Catana.

**Once in a while, users will receive email reminders about their TODOs.**

### <mark style="color:blue;">Expiring TODOs</mark>

{% hint style="info" %}
The main purpose of expiring TODOs is **helping write temporary chunks of code.**
{% endhint %}

When introduced in a codebase, a TODO should never be a priority. If it were, using a TODO would not be appropriate. However, it may become a priority at a later point.\
\
Software engineers frequently have to work on tasks requiring a multi-step process.\
For instance, modifying or renaming a background job. The changes needs to be backward compatible until the queue is drained from the previous job's version.&#x20;

<figure><img src="../.gitbook/assets/job-one-step.png" alt="" width="563"><figcaption><p><strong>Renaming a job in a single step will create an outage.</strong></p></figcaption></figure>

<figure><img src="../.gitbook/assets/job-two-steps.png" alt="" width="563"><figcaption><p><strong>User has to remember to remove the old job.</strong></p></figcaption></figure>

When a **TODO expires it effectively becomes an actionable issue**. Therefore, instead of sending an email reminder, **Catana opens a ticket in your project management tracker.** This allows its  author and team members to prioritise and address the issue as they see fit.

<figure><img src="../.gitbook/assets/drain-queue.png" alt="" width="563"><figcaption><p><strong>Using an expiring TODO helps surface it when it expires.</strong></p></figcaption></figure>

Expiring a TODO doesn't have to be at a specific date in the future. Whether you need to address a TODO when a related bug is fixed or when a dependency you rely on gets upgraded, **Catana offers various triggers to help you surface and prioritize tasks** at the right moment.



