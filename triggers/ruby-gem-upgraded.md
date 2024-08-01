# Ruby Gem upgraded

{% hint style="info" %}
Use the Ruby Gem upgraded trigger to expire a TODO **when a version of a Gem matching the constraint(s) is upgraded in your application**.
{% endhint %}

<figure><img src="../.gitbook/assets/gem-bump.png" alt="" width="563"><figcaption></figcaption></figure>

### Usage

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`gem_bump`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'nokogiri', '> 1.15'`**</mark>**`))`**

### Examples

<details>

<summary>Expire a TODO when  Nokogori is upgraded in your application with a version '<code>> 1.15'</code></summary>

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`gem_bump`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'nokogiri', '> 1.15'`**</mark>**`))`**

</details>

<details>

<summary>Expire a TODO when Rails is upgraded in your application to version 7.1</summary>

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`gem_bump`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'nokogiri', '7.1'`**</mark>**`))`**

</details>

<details>

<summary>Expire a TODO when Devise is upgraded in your application with a version '<code>> 4.9.2'</code> and <code>'&#x3C; 5'</code></summary>

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`gem_bump`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'devise', '> 4.9.2', '< 5'`**</mark>**`))`**

</details>
