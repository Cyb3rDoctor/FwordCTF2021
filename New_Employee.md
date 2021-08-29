# New Employee (OSINT - 1000 points)

![image](https://user-images.githubusercontent.com/70543460/131232583-83c6d673-01c1-4df9-bd0f-742796939b67.png)

---



Notes:

1. I'll add more details in some steps soon.

2. A lot of skills/techniques from several intelligence disciplines/sub-disciplines are included in this challenge (OSINT, SOCMINT, IMINT and GEOINT).



-------------------------------------------------- 

## [1] Identifying the scope: 

I gave you a name (Qunnoune Phrasavath) in the challenge description, so what you need to do is to search for that name in the popular social media sites and you'll find that he has accounts on 3 of the popular photos-sharing social media platforms ( Instagram, Pinterest and Flickr). 

1. https://www.instagram.com/qunnoune/

![image](https://user-images.githubusercontent.com/70543460/131240126-c5e75b87-1b1d-4d2a-a361-871dac3179f5.png)

2. https://www.pinterest.com/qunnoune/

![image](https://user-images.githubusercontent.com/70543460/131240137-1227ed70-533b-4304-875c-d55d549ea7b8.png)

3. https://www.flickr.com/photos/193766884@N07/

![image](https://user-images.githubusercontent.com/70543460/131240154-c6f583c1-de69-4798-a89d-5535fd8c7095.png)

<br/><br/>
**Noting that all of the above accounts have the same username and the same profile picture**
<br/><br/>

Some things you may ask about: 

1) I can't find him when I google his name! ==> **That's intended.**

2) What about the Github account? ==> **I've sent a notification on the CTF site and pinned a message in the OSINT channel in the CTF Discord server to inform competitors that the Github account is fake. I also answered everyone who asked me to confirm any account.**

3) Are you sure that we're not targeting a real person? ===> **Yes.**

-------------------------------------------------- 

## [2] Analyzing the found accounts:

### Instagram:

You'll only find 1 post in the Instagranm account that says:
Hi, this is my new account on: Instagram

![image](https://user-images.githubusercontent.com/70543460/131239938-c3d2ec8f-55f0-4f37-8247-82c12298fd96.png)
<br/><br/>
### Pinterest:

You'll find a total of 3 pins in 2 boards, the first board is called "Pictures" and it contains 1 picture that says:
Hi, this is my new account on: Pinterest

And the other board is called "Going to Work", and it contains 2 images of 2 places.

![image](https://user-images.githubusercontent.com/70543460/131239982-52842596-450b-4289-8bb6-dfddd9d7e159.png)
<br/><br/>
### Flickr:

You'll find a total of 6 images posted there. One of them says:
Hi, this is my new account on: Flickr

And the 5 other images are for 5 places.

![image](https://user-images.githubusercontent.com/70543460/131240016-56561a9f-63e9-4380-b85e-cfee073338de.png)


-------------------------------------------------- 

## Notes after the second step:

1. "Hi, this is my new account on: (platform name)". ==> As those are his ""new"" accounts, he probably had old accounts on the same platforms as he posted the same picture that says that the account is new on each one of them.

2. Flickr has the most number of pictures. ==> This was intended to be a clue that clarifies that he uses Flickr more then Pinterest and more than Instagram.

3. All of the social media platforms he uses are for photo-sharing.

-------------------------------------------------- 

## [3] Geolocating the images:

It's clear according to the board name in Pinterest / the album name in Flickr (Road to Work) that those images are related to the location of the company where he works.

<br/><br/>

Notes:
1) This step requires using some IMINT techniques, such as Reverse Image Searching in order to find the locations of the pictures.
2) You can use the IMINT techniques/skills to locate one image then check the street view and you'll find that all the locations are near each other, or you can use the IMINT techniques/skills to locate each one of them then add then check the destination between all of them and you'll also find that all the locations are near each other...

```
**I'll explain how to locate one image using some IMINT techniques/skills and add that to the writeup soon**
```

Note: Here are the images sources:

https://www.google.com/maps/@40.8122636,-73.920619,3a,45y,301.09h,97.26t/data=!3m6!1e1!3m4!1snWbMYIxCkpCHV7RxiGZwpg!2e0!7i16384!8i8192


https://www.google.com/maps/@40.8132685,-73.9228067,3a,75y,325.31h,150.46t/data=!3m6!1e1!3m4!1sDRDd49ChGwlQoP03mc2mBQ!2e0!7i16384!8i8192


https://www.google.com/maps/@40.8125469,-73.9233381,3a,75y,55.39h,145.71t/data=!3m6!1e1!3m4!1sm88p6GVTQs7y7zupof_zZA!2e0!7i16384!8i8192


https://www.google.com/maps/@40.8110699,-73.9215372,3a,75y,298.86h,117.27t/data=!3m6!1e1!3m4!1sCzgHJopPKwQo4jZ1037HMw!2e0!7i13312!8i6656

https://www.google.com/maps/@40.8119732,-73.9236622,3a,29y,23.48h,93.79t/data=!3m7!1e1!3m5!1seEqXRUgy9I_KLOz7hiWIBA!2e0!6shttps:%2F%2Fstreetviewpixels-pa.googleapis.com%2Fv1%2Fthumbnail%3Fpanoid%3DeEqXRUgy9I_KLOz7hiWIBA%26cb_client%3Dmaps_sv.tactile.gps%26w%3D203%26h%3D100%26yaw%3D90.58028%26pitch%3D0%26thumbfov%3D100!7i16384!8i8192


<br/><br/>

![image](https://user-images.githubusercontent.com/70543460/131242399-2722fd93-5dc0-4d08-a3c2-0724dc509f98.png)
 

-------------------------------------------------- 

## [4] Linking everything together:


According to the notes I mentioned above:

```
1. "Hi, this is my new account on: (platform name)". ==> As those are his ""new"" accounts, he probably had old accounts on the same platforms as he posted the same picture that says that the account is new on each one of them.

2. Flickr has the most number of pictures. ==> This was intended to be a clue that clarifies that he uses Flickr more then Pinterest and more than Instagram.

3. All of the social media platforms he uses are for photo-sharing.
```

And according to the scenario of the challenge (The challenge asks for an employee serial number):

The target (Qunnoune Phrasavath) may have posted something also related to his work on one/all of his old accounts.

..

One of the important skills in SOCMINT is understanding the features of the social media platforms that you're targeting, because that will help you in navigating and using them in a proper way in your inverstigation.

So, your task is to do some researche about the features of Instagram, Pinterest and Flickr as all of them are used by the target.

..

To conclude the final step, you'll find that one of the features of Flickr is something called "Flickr Map" (https://www.flickr.com/map)

https://startuptalky.com/what-is-flickr-how-works/
![image](https://user-images.githubusercontent.com/70543460/131242873-c5502e74-be2f-4f9a-b280-8009d75b59e5.png)

<br/><br/>

So, after going to the area of the posted images, you will find one photo located in the middle of the area of the locations that you have found from the photos on the target's social media accounts:

![image](https://user-images.githubusercontent.com/70543460/131243090-cac97af2-d553-422d-832e-7633a159a0b0.png)

<br/><br/>

https://www.flickr.com/photos/193731128@N05/51397189261
![51397189261_8f31f38a14_o (2)](https://user-images.githubusercontent.com/70543460/131243186-e0a4a158-136d-4244-84a4-16bbaaac7613.jpg)

<br/><br/>

**The ID card of "Qunnoune Phrasavath" appears in the picture with a PDF417 barcode that will reveal his serial number

![image](https://user-images.githubusercontent.com/70543460/131243330-2bbda4bd-c58b-4e33-8133-08b673fb97c7.png)

![image](https://user-images.githubusercontent.com/70543460/131243492-a7f2dcf9-ac03-4266-88f6-77ebe718cf3b.png)


----------------------------------------------------------------------------------------------------

# This challenge was inspired from 2 real stories:

"Keeping the location tags in the metadata of the picture" was inspired from:

https://www.npr.org/sections/thetwo-way/2012/12/04/166487197/betrayed-by-metadata-john-mcafee-admits-hes-really-in-guatemala



"Posting a picture that leaks some information by mistake" was inspired from:

https://newsbeezer.com/romaniaeng/defense-ministers-mistake-nicolae-ciuca-accidentally-posted-access-passwords-for-an-army-call-center-on-facebook/
