# GitHub Issue closed

{% hint style="info" %}
Use the GitHub issue closed trigger to expire a TODO when a **GitHub issue is closed.**
{% endhint %}

<figure><img src="../.gitbook/assets/issue-close.png" alt="" width="563"><figcaption></figcaption></figure>

### Usage

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`issue_closed`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'rails', 'rails', 631`**</mark>**`))`**

### **Authorization**

This trigger can be used to monitor issues on any **public repositories or private repositories belonging to the same organization the TODO is introduced.**

### Examples

<details>

<summary><em>Expire a TODO when the issue #631 from the Rails repository is closed</em></summary>

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`issue_closed`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'rails', 'rails', 631`**</mark>**`))`**

</details>
