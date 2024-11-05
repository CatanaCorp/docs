# Ruby Version upgraded

{% hint style="info" %}
Use the Ruby upgrade trigger to expire a TODO **when Ruby is upgraded in your application to a new version.**
{% endhint %}



<figure><img src="../.gitbook/assets/Ruby bump trigger.png" alt=""><figcaption></figcaption></figure>

### Usage with a syntax

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`ruby_bump`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`[...]`**</mark>**`))`**

### Requirements

Catana detects the ruby version your application runs on by parsing the `Gemfile.lock` file.\
Pull Requests introducing a TODO with a `ruby_bump` trigger will [fail validation](../core-concepts/validation.md) in the following conditions:

* Your application does not have a `Gemfile.lock` file.
* The `Gemfile.lock` file is **not** located at the root of your project.
* The `Gemfile.lock` file lacks Ruby Version information because the `Gemfile` doesn't [specify a Ruby Version](https://bundler.io/guides/gemfile\_ruby.html).

#### Examples

<details>

<summary>Expire a TODO when Ruby is upgraded to a version superior to the current one.</summary>

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`ruby_bump`**</mark>**`)`**

</details>

<details>

<summary>Expire a TODO when Ruby is upgraded to version 3.3 or higher.</summary>

➡️ **`TO`**➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`ruby_bump`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'> 3.3'`**</mark>**`))`**

</details>

<details>

<summary>Expire a TODO when Ruby is upgraded to 3.2.2</summary>

➡️ **`TO`**➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`ruby_bump`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'3.2.2'`**</mark>**`))`**

</details>

### Usage when detected automatically

#### Examples

<mark style="color:blue;">TODO</mark>:  **Use the new Regexp timeout feature once we are on Ruby 3.2**\
<mark style="color:orange;">Equivalent to</mark>: <mark style="color:yellow;background-color:yellow;">**`ruby_bump`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'3.2'`**</mark>**`)`**

<mark style="color:blue;">TODO</mark>:  No need to remove the tempfile manually on Ruby 3.4, if we use the anonymous keyword\
<mark style="color:orange;">Equivalent to</mark>: <mark style="color:yellow;background-color:yellow;">**`ruby_bump`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'3.4'`**</mark>**`)`**

<mark style="color:blue;">TODO</mark>:  Do something after we upgrade Ruby\
<mark style="color:orange;">Equivalent to</mark>: <mark style="color:yellow;background-color:yellow;">**`ruby_bump`**</mark>**`()`**
