# R_Time_Capsule
This is a Full Application with Web, Mobile and BackEnd!

## How Wdoes it works? 
The Application goal is to deliver to the user a time capsule, with the date, image and description of the memory that the user might want to insert to its Time Capsule. It counts with a Mobile and a Web version.

Both the Mobile or Web versions work the same way. In the home page, the user needs to sincronize with a GitHub account. Then, when the user is properly logged in, it will show the options of logging out the application, creating a new memory or showing the memories that was already created before (if there is no memory, the page will be blank).

If the user chooses to log out, the GitHub account login token will be saved into cookies that expires in 30 days for posterior re-login. After the 30 days, the token will be reseted and ask to the user to login again manually and save another token for other 30 days. And so it goes. 

If the user already loged in and already created memories before, the memories already created will be shown right after the login. if the momories does not exists, then the 'create memories' option will be shown first.

To create memories, the user might insert an image, a description to the memory and whether if it is a public or a private memory. The date of inserction of the memory is automatic.

As said before, after the memory is created, it will be shown in the 'memories' page with all the proper information inserted.

## How was is developed?
It was developed using React, Next.js, Express and TypeScript. In addition to other technologies.



