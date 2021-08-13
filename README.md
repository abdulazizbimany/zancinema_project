# ZANCINEMA WEB APPLICATION PROJECT
A Zancinema project, is a final project of the Interactive Website Development course from The State university of Zanzibar (SUZA) that was done by Abdulaziz Said Soud as a student of diploma for Computer Science in that University and other three members (newbie programmers).


*********** **End** **User** **Section** (**FRONT**) ***********
path: zancinema/index.php

This project is a dynamic web cinema booking system that allows an end user to signup, login
and book the movie show that is in the current shows of the week at zancinema. A user can also
see coming soon movies at Zancinema, he can also open the about us page and the contact page
to contact with zancinema or locate them on google map.

The end user must signup if he/she was  not signup before to the system, and login if he want to book.

Due to the time of the semester and the scope of the project is complex to my fellow newbie
developers we could not be able to implement the end user panel to see his/her current bookings
and booking history.


********* **Staff**/**Admin** **Section** (**BACK**) *********
path: zancinema/admin/index.php

The system allows the admin to login and manage homepage, about page, contact page, bookings, contacts,
users, my profile and report.

After 10 Minutes of inactive, for the security purpose the system destroys the session and the admin must
login again.

On every page that an admin can upload image, even if he opened that page to change other details and not
image, he must re-upload the image before click the submit button. Yes, this is the bug that needs to be
fixed but for the time we build the system, there were alot of things to learn and focus on upgrading
the features of the system so we forgot to fix this bug.

Another bug is, you can't delete user that was booked because we have used the primary key of the user as
the foreign key on bookings table.

As we implemented a high security technique method for the password that stored in the system, it may be
not possible to check or change the password on phpMyAdmin panel even if you try different algorithms of
encryption on it like (md5, Sha1 etc).

**The** **credentials** **for** **an admin/staff login are:**
email: admin@admin.com
password: 123

The password like 123 is not the password that is stored in Database instead, the system takes that 123 and
encrypt it by using md5 algorithm that returns 32 bit characters, combine the first and last encrypted
peppers defined by the sytsem and and hash them by using GOST algorithm that returns 64 bit characters.

**Formula:**
hash('gost', (md5(firstPepper) + md5(realPassword) + md5(lastPepper)))

--------------------- **I'M PROUD AND GAINED ALOT OF KNOWLEDGE ON THIS DYNAMIC WEB PROJECT!**---------------------------
                                                   **Thank You!**

**GROUP NO 2**
1. ABDULAZIZ SAID SOUD (Leader)
2. HUSSEIN KHEIR MAKAME
3. OMAR MKUBWA OMAR
4. SALIM MAULID SALUMS


