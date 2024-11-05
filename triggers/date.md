# Date

{% hint style="info" %}
Use the date trigger to **expire a TODO at a specified date**.
{% endhint %}

<figure><img src="../.gitbook/assets/date-trigger.png" alt="" width="563"><figcaption></figcaption></figure>

### Usage with a syntax

➡️ **`TODO(on:`**<mark style="color:yellow;background-color:yellow;">**`date`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'2023-06-01'`**</mark>**`))`**\
➡️ **`TODO(on:`**<mark style="color:purple;background-color:purple;">**`'2023-06-01'`**</mark>**`)`** (Same as above, but with the short form)

#### Examples

<details>

<summary><em>Expire a TODO on June 1st, 2023</em></summary>

➡️ **`TODO(on:`**<mark style="color:purple;background-color:purple;">**`'2023-06-01'`**</mark>**`)`**&#x20;

</details>

<details>

<summary><em>Expire a TODO on August 23rd, 2023 at 10AM</em></summary>

➡️ **`TODO(on:`**<mark style="color:purple;background-color:purple;">**`'2023-08-23 10:00'`**</mark>**`)`**&#x20;

</details>

### Usage when detected automatically

Catana will always use today's date as reference point for relative dates (next month, in three weeks...).\
You can omit some components from a date (the day, month or year), in such cases Catana will fill itself, **with the final result being a date always in the future.**\
\
Catana will never detect a date trigger if the date you specify is undetermined (later, someday, when I have time ...).

#### Examples

<mark style="color:blue;">TODO</mark>:  **Ensure we use the blob package by Feb. 4**\
<mark style="color:orange;">Equivalent to</mark>:  <mark style="color:yellow;background-color:yellow;">**`date`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'2025-2-4'`**</mark>**`)`**  (Assuming today's date is passed Februry 4)

<mark style="color:blue;">TODO</mark>:  **Tweak the debounce next week once we have collected enough real traffic data**\
<mark style="color:orange;">Result</mark>:  <mark style="color:yellow;background-color:yellow;">**`date`**</mark>**`(`**<mark style="color:purple;background-color:purple;">**`'2024-11-12'`**</mark>**`)`**  (Assuming today's date is November 5)

<mark style="color:blue;">TODO</mark>:  Polish and optimise after hack days\
<mark style="color:orange;">Result</mark>:  _No detection, as the event's date can't be determined._
