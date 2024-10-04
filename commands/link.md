# Link

{% hint style="info" %}
The **`@CatanaCorp link`** command can be invoked by commenting on a Pull Request.
{% endhint %}

#### <mark style="color:blue;">When to use it</mark>

A common convention is to require each TODO to have an associated issue, with the TODO referencing the issue number.\
This workflow is tedious, as developers need to manually create an issue for each TODO, update the codebase to link the issue number, commit the changes, and finally push to Git.

**Catana automates this process, saving you and your team valuable time.**

#### <mark style="color:blue;">Command</mark>

➡️ **`@catanacorp`**<mark style="color:purple;">**`link`**</mark>

This command performs the following actions:

* Parses the Pull Request changes and detects new TODO annotations.
* Opens a GitHub issue for each new TODO item.
* Edits each TODO in the codebase to reference the corresponding issue. The changes made by the Catana bot are not pushed to your branch but are provided as GitHub suggestions, which you can apply with a single click.

<figure><img src="../.gitbook/assets/Link example.png" alt=""><figcaption></figcaption></figure>
