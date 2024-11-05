# Ruby Gem released

{% hint style="info" %}
Use the Ruby Gem released trigger to expire a TODO **when a version of a Gem matching the constraint(s) is released**.
{% endhint %}

<figure><img src="../.gitbook/assets/gem-release.png" alt="" width="563"><figcaption></figcaption></figure>

### Usage with a syntax

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`gem_release`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'nokogiri', '> 1.15'`**</mark>**`))`**

#### Examples

<details>

<summary>Expire a TODO when the Nokogori Ruby gem is released with a version '<code>> 1.15'</code></summary>

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`gem_release`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'nokogiri', '> 1.15'`**</mark>**`))`**

</details>

<details>

<summary>Expire a TODO when the Rails Ruby gem version 7.1 is released</summary>

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`gem_release`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'nokogiri', '7.1'`**</mark>**`))`**

</details>

<details>

<summary>Expire a TODO when the Devise Ruby gem is released with a version '<code>> 4.9.2'</code> and <code>'&#x3C; 5'</code></summary>

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`gem_release`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'devise', '> 4.9.2', '< 5'`**</mark>**`))`**

</details>

### Usage when detected automatically

Please ensure you always explicitly mention the term "gem" (literally), for Catana to correctly detect this trigger.

#### Examples

<mark style="color:blue;">TODO</mark>:  **Make sure to upgrade when the gem super-fun is released to 3.5.1**\
<mark style="color:orange;">Equivalent to</mark>: <mark style="color:yellow;background-color:yellow;">**`gem_release`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'super-fun', '3.5.1'`**</mark>**`)`**

<mark style="color:blue;">TODO</mark>:  **Check the required redis-rb version once the sidekiq gem gets a new release in the > 7 serie**\
<mark style="color:orange;">Equivalent to</mark>: <mark style="color:yellow;background-color:yellow;">**`gem_release`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'sidekiq', '> 7'`**</mark>**`)`**

<mark style="color:blue;">TODO</mark>:  **Do something after kuaz-thermometer cuts 3.4**\
<mark style="color:orange;">Equivalent to</mark>:  _No detection as the term "gem" is not mentioned_
