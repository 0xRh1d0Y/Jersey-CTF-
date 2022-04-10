# Jersey-CTF
Write-up for Jersey CTF challenges.

## :clipboard: Table of Contents

- [:triangular_flag_on_post: Osint](#triangular_flag_on_post-osint)
- 
## :triangular_flag_on_post: Osint

### Problem's Name :***Dnsjoke***

### Problem Description:

![image](https://user-images.githubusercontent.com/79222856/162631983-a6efc5e0-d2df-4b5c-9f6f-42b8264c1df6.png)

### Solution:

![image](https://user-images.githubusercontent.com/79222856/162632261-4aa3940e-bb3c-496a-9460-86b471641341.png)


### Explanation:

After reading the description i realised its a dns realted problem!
So, Let's go to the site viewdns and search for dns record lookup 
with the domain name that provided in the description.Then i check
the result and yes i found the flag.

**Here is the [link](https://viewdns.info/dnsrecord/?domain=jerseyctf.com) of viewdns result.


### Summary:
Flag: "jctf{DNS_J0k3s_t@k3_24_hrs}"
