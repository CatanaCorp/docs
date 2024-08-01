# GitHub Pull Request closed

{% hint style="info" %}
Use the GitHub Pull Request closed trigger to expire a TODO when a **GitHub Pull Request is closed.**
{% endhint %}

<figure><img src="../.gitbook/assets/pr-close.png" alt="" width="563"><figcaption></figcaption></figure>

### Usage

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`pr_closed`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'lodash', 'lodash', 44`**</mark>**`))`**

### **Authorization**

This trigger can be used to monitor pull requests on any **public repositories or private repositories belonging to the same organization the TODO is introduced.**

### Examples

<details>

<summary><em>Expire a TODO when the Pull Request #44 from the lodash repository is closed</em></summary>

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`pr_closed`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'lodash', 'lodash', 44`**</mark>**`))`**

</details>
