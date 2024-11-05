# Overview

<figure><img src="../.gitbook/assets/trigger-example.png" alt="" width="563"><figcaption></figcaption></figure>

Catana provides a powerful feature to **expire your TODO at the time or condition of your choice by using triggers.** \
**When the condition of the trigger is met, Catana expire your TODO and open an issue in your GitHub tracker.**

{% hint style="info" %}
The [Core concept](../core-concepts/regular-and-expiring-todos.md) page has a detailed explanation on expiring TODOs.
{% endhint %}

### Usage

Adding a trigger to a TODO can be done in two ways, **using a specific syntax** on the TODO declaration or let Catana **detect it itself with its fine tuned AI model (currently in beta)**.

#### With a syntax

<figure><img src="../.gitbook/assets/trigger-anatomy.png" alt=""><figcaption></figcaption></figure>

The parser expects the following syntax: TODO(<mark style="color:green;background-color:green;">**on**</mark>: <mark style="color:yellow;background-color:yellow;">**date**</mark>(<mark style="color:purple;background-color:purple;">**'2023-06-01'**</mark>)).\
For more examples, each trigger type has its own documentation page. Do not worry if you make a mistake; Catana will provide feedback on your pull request!

#### Let Catana use its fine tuned AI model

<figure><img src="../.gitbook/assets/Date trigger with AI.png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
This feature is currently in beta; you can opt in by heading to your repository's settings page on the Catana dashboard.\
\
Please allow for some margin of error if the trigger is either not detected at all or the wrong trigger is used.
{% endhint %}

The prompt used to detect the trigger is based on the TODO title. For instance, if you'd like the TODO to expire when your application upgrades its Ruby version, you would write:\
\
`TODO: Use the Regex timeout feature once we are on Ruby 3.2`

Another common example is to expire a TODO and follow up on a task when a related pull request or issue is closed:

`TODO: Reuse the calendar component once #5413 is merged`

***

The next pages in the documentation go through all triggers implemented by Catana and provide examples on how to help the AI model detect the correct trigger.

### CI feedback

In addition to the [validation feature](../core-concepts/validation.md), when opening a pull request, Catana will output all details of the TODOs it detected and the operations it will perform once your commit(s) land on the main branch.

This is especially useful if you'd like to know in advance which trigger Catana inferred from a TODO. The details are viewable on your pull request's check run page.

<figure><img src="../.gitbook/assets/Ci Check output.png" alt=""><figcaption></figcaption></figure>

