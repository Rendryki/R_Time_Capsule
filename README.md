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
It was developed using React, Next.js, Fastify and TypeScript. In addition to other technologies.

The Web Development used React and Nextjs. The Mobile development used React Native. The Backend development used Express and TypeScript. Also, the application used TailWindCSS along side with other technologies, libraryes and tools.

The Web Application was developed in TypeScript along with React and Next.Js. So, the routing on the web page is totally handled by Next.Js. All the data showed is fetched from the own application database. All the data inserted by the user is inserted in the own app database either. The GitHub account is loged in throwgh Oauth authentication. The Oauth authorization token is saved by cookies for a limited period of time. After the cookie expires, another login that generates another token for another 30 days is necessary.

The Mobile App was also developed using TypeScript, but together with React Native and Expo. Routing in the mobile app is completely handled by the Expo tools for React Native. All the data showed is fetched from the own application database. All the data inserted by the user is inserted in the own app database either. The GitHub account is loged in throwgh Oauth authentication. The Oauth authorization token is saved by a cookies handler forneced by Expo. Those autentication token are not expireble in the Mobile App. 

The Backend was developed using TypeScript and Node.js. It was used Fastify to handle the comunication with the Database and the routing inside the Backend. Also, the app used Axios to communicate with GitHub and get the login Oauth authorization. Axios was also used in the Mobile and Web to comunicate with the backend server.
The Database communication happens with Prisma Studio contribution. It is a relational database and its query was written with the support of Prisma.

Last but not least. All of the application development process occurred together with the 'Next Level Week' event offered by Rocketseat in their own platform. It can be accessed by the following URL: https://app.rocketseat.com.br
