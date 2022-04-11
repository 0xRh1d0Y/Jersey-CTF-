# Jersey-CTF
Write-up for Jersey CTF challenges.

## :clipboard: Table of Contents

- [:triangular_flag_on_post: Osint](#triangular_flag_on_post-osint)
- - [:triangular_flag_on_post: Dnsjoke](#triangular_flag_on_post-dnsjoke)
- - [:triangular_flag_on_post: Photo-op-spot](#triangular_flag_on_post-photo-op-spot)
- [:triangular_flag_on_post: Web](#triangular_flag_on_post-web)
- - [:triangular_flag_on_post: Heres-my-password](#triangular_flag_on_post-heres-my-password)

## :triangular_flag_on_post: Osint

## :triangular_flag_on_post: Dnsjoke

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



## :triangular_flag_on_post: Photo-op-spot

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

Step 1: Reverse Image Search

First of all, I tried reverse image search and found the address 132 Minor Ave N !
I thought that i found the address of that image and tried it  like jctf{Minor-Ave-N}
but it was wrong!.Then one of my teammate said that it can be solve by what3word website !
Ah snap! he was right.After searching with the address,
Finaly we got the right flag that the place adress repesent by three word.

Step 2: what3word 

Then in the what3word site search with the address 132 Minor Ave N .Then i found the name of the picture  Public Art "TransForest" in the map!.Then clicked the location of the picture of the name and found three word  that represent the  location .

***Here the [Link](https://what3words.com/unwanted.debate.wake) of the what3word site result.

### Summary:

Flag : "jctf{unwanteddebatewake}"



## :triangular_flag_on_post: Web

## :triangular_flag_on_post: Heres-my-password

### 3.Problem's Name :***heres-my-password***

### Problem Description:

![image](https://user-images.githubusercontent.com/79222856/162687398-640eaa29-f560-4f59-9119-bf9de8730148.png)

### Problem Hint:

![image](https://user-images.githubusercontent.com/79222856/162687568-c6fc8917-ae28-4e07-846d-8bed38ba841a.png)

### Solution && Explanation:

From the description we understand that we need to bruteforce the a login page.
And they provide us a users.txt file which contains 500 username and they also give
only one password. We need to bruteforce 500 usernames with just one password and 
have to find right user!.For this  bruteforce attack I start my  burpsuite!

    Step 1: First intercept the request.

![image](https://user-images.githubusercontent.com/79222856/162688531-a1c71c90-dace-4823-961b-ca50d5049a49.png)

![image](https://user-images.githubusercontent.com/79222856/162689023-4810bff5-a869-42e6-997b-8e7d1dd06d30.png)

    Step 2: Send the request to intruder.

![image](https://user-images.githubusercontent.com/79222856/162689212-d1adf008-aa0b-48a3-abac-e5b45a2f5145.png)

    Step 3:
     
    Then go to the position tab and click on the Clear button.
    This will clear default selection.After clearing default
    selection select only username and click on the Add button 
    to bruteforce. This will select only username .And select
    the Attack type to Sniper.
    
<br>
    
    Step 4: Go to the Payload tab.
    
![image](https://user-images.githubusercontent.com/79222856/162690687-f5e472c5-bb6c-4468-bce8-0d630071b25e.png)


    Step 5:
    
    You will see that the sniper attack type have only one 
    paylode set/payload type. Load the payload type of  
    simple list with the 500 usernames. To do that click 
    the Load button and find the users.txt file. After 
    that click on Start Attack to start the bruteforce attack.
    
![image](https://user-images.githubusercontent.com/79222856/162691504-90f45fbe-8c8a-4f03-bf54-f6aeeb8cdb4c.png)


    Step 6:
    
    See there is a lot of response with same status code.
    So how do we know the correct response? By simply 
    clicking on the Length button twice you will see 
    the different length 798.Here the username Wolverine.
    Now let’s see the full  response of that request. 
    You can see the flag.
    
![image](https://user-images.githubusercontent.com/79222856/162691890-49d20671-880b-424f-b458-1560afff9447.png)

![image](https://user-images.githubusercontent.com/79222856/162692625-045ee0f4-1f27-437a-848b-6e6c0128177d.png)


### Summary:
```
Flag:- jctf{c0NGR@T2_y0U_p@22wORd_SPR@y3D!}

```

    
    
    
