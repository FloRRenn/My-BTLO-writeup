# Squid Game
**#CTF** **#OSINT** **#Analyze** **#DigitalForensics**

[My achievement](https://blueteamlabs.online/achievement/share/challenge/68894/33)

---

## 1. Scenario
Will you survive the Squid Games?

## 2. Challenge
You got an [invitation card](./img/Invitation%20Card.jpg), then you has to find hidden information arround it. This is provided invitation card:

![invitation card](./img/Invitation%20Card.jpg)

### Q1. What is the phone number on the invitation card in Squid Game? (Research this online!)
Hint: The phone number is not stored in the invitation card. You need to use your **OSINT skill** to find it.
P/S: I attempted to use some phone numbers that I found on the internet before finally getting the correct one.

<details>
<summary>Answer</summary>

```
*******6
```
</details>

### Q2. Can you extract something from the invitation card file? What is the name of the file?

Hint: Once you have the phone number, it will serve as the password to extract a hidden file stored within the invitation card. You can use tool like `steghide` to do that.

<details>
<summary>Answer</summary>

```
The hidden file type is an image
```
</details>

### Q3. What hint text can be discovered in the final file?
Hint: To reveal the hidden file, utilize tools such as `Stegsolve.jar` which allows you to adjust the color of the hidden file. The hidden text will only be visible when you switch to the correct color mode.

<details>
<summary>Answer</summary>

```
*** *****
```
</details>

### Q4. What is the final flag?
Hint: The answer from Q3 is a clue. Search for something weird in the hidden image using this clue. Once you've found it, extract it using tools like [pixspy](https://pixspy.com/) (which I discovered while seeking hints on Discord) or code a tool to do that. Then you should find the relationship between them.

<details>
<summary>Answer</summary>

```
- These weird things are very very small. 
- Several transformations (decode) with these weird ones are required to obtain the final flag.

The flag is SBT{**************}
```
</details>