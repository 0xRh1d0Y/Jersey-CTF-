# Jersey-CTF
Write-up for Jersey CTF challenges.

## :clipboard: Table of Contents

- [:triangular_flag_on_post: Osint](#triangular_flag_on_post-osint)
- 
## :triangular_flag_on_post: Osint

### 1.Problem's Name :***Dnsjoke***

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





### 2. Problem's Name :***photo-op-spot***

### Problem Picture:

![image](https://user-images.githubusercontent.com/79222856/162636706-e9e82f13-b581-492f-af55-8ba2c55cff54.png)


### Problem Description:

![image](https://user-images.githubusercontent.com/79222856/162636567-40fa77cc-7f04-4cee-8219-497f9058d193.png)


### Problem Hint:

![image](https://user-images.githubusercontent.com/79222856/162636736-3a2b1aac-e7b7-4f9d-a86b-a4580e3e008a.png)

### Solution:

Reverse Image Search:

![image](https://user-images.githubusercontent.com/79222856/162636783-52df47e6-601d-4cc2-b3de-8207676ee7a0.png)

![image](https://user-images.githubusercontent.com/79222856/162636848-3f9c9881-a6ce-48c9-b883-84577b225d72.png)

![image](https://user-images.githubusercontent.com/79222856/162637024-8846c1fb-203c-4dea-a8ce-ef21a69136cc.png)

![image](https://user-images.githubusercontent.com/79222856/162637063-348d3e5c-5933-4bb8-af2e-87c8d5a76c45.png)

![image](https://user-images.githubusercontent.com/79222856/162637078-1e8541fd-58d8-4439-a8f9-d571807bb631.png)

![image](https://user-images.githubusercontent.com/79222856/162637118-b7d396fe-3f68-4463-bba5-4241a3e77d3e.png)

![image](https://user-images.githubusercontent.com/79222856/162637194-1067a0fa-f0bc-4a4e-a54d-5e8fa04937a2.png)


### Explanation:

First of all, I tried reverse image search and found the address 132 Minor Ave N !
I thought that i found the address of that image and tried it  like jctf{Minor-Ave-N}
but it was wrong!.Then one of my teammate said that it can be solve by what3word website !
Ah snap! he was right.After searching with the address,
Finaly we got the right flag that the place adress repesent by three word.

***Here the [Link](https://what3words.com/unwanted.debate.wake) of the what3word site result.
### Summary:

Flag : "jctf{unwanteddebatewake}"

