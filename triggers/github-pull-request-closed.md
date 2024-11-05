# GitHub Pull Request closed

{% hint style="info" %}
The GitHub Pull Request closed is an alias to the [GitHub Issue closed trigger.](github-issue-closed.md)
{% endhint %}

<figure><img src="../.gitbook/assets/pr-close.png" alt="" width="563"><figcaption></figcaption></figure>

### Usage with a syntax

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`pr_closed`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'lodash', 'lodash', 44`**</mark>**`))`**

### **Authorization**

This trigger can be used to monitor pull requests on any **public repositories or private repositories belonging to the same organization the TODO is introduced.**

#### Examples

<details>

<summary><em>Expire a TODO when the Pull Request #44 from the lodash repository is closed</em></summary>

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`pr_closed`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'lodash', 'lodash', 44`**</mark>**`))`**

</details>

### Usage when detected automatically

When the repository or organisation is not specified, Catana will assume you are referring to a Pull Request in the current repository.

#### Examples

<mark style="color:blue;">TODO</mark>:  **Skipping this test until we fix #881**\
<mark style="color:orange;">Equivalent to</mark>: <mark style="color:yellow;background-color:yellow;">**`pr_closed`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'org', 'repo', 881`**</mark>**`)`**

