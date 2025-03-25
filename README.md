## 🚀 SS-Connect: Instant Messaging Application  

SS-Connect is an instant messaging application designed to connect people with different interests and facilitate collaboration on projects.  

The application was developed using **Angular 16 and Firebase** and includes the following features:  

- **Home page** to explore profiles and connect with other users.  
- **Profile section** where users can view their information.  
- **Registration and login system** for secure access.  
- **Real-time messaging** that allows conversations with multiple people.  
- **Interactive feedback**, including notifications for account creation, incorrect passwords, and non-existent users, among others.  

## 📷 Screenshots  
Displaying available user profiles.
![available user profiles](/src/assets/images/main-users.png)
User information profile.
![user information profile](/src/assets/images/page-profiles.png)
Real time conversations between users.
![messagin page](/src/assets/images/messaging.png)

## 🖥 Installation and Setup  

#### Prerequisites  
Before starting, make sure you have:  

- A **code editor** installed.  
- A **Firebase account** with **Authentication** and **Firestore Database** enabled.  

#### Installation  
Clone this repository and open the project in your code editor.

Install the required dependencies:  

```bash
npm install
```

#### Configuration  
Add the **API KEY** provided by Firebase to the environment variables:  

```tsx
export const environment = {
  production: false,
  firebase: { // Add your API KEY information here
    apiKey: "",
    authDomain: "",
    projectId: "",
    storageBucket: "",
    messagingSenderId: "",
    measurementId: ""
  },
};
```

#### Running the Application  
To start the server, run:  

```bash
ng serve
```

To access the application, open:  

```
http://localhost:4200/login
```

## 🖋 Reflection  

The main objective of this application was to **connect people with diverse skills to collaborate on interdisciplinary projects** while also exploring and adapting to technologies such as **Angular and Firebase**.  

The development process posed several challenges. Navigation and authentication required implementing access restrictions to prevent users without accounts from entering restricted sections. Real-time messaging was another major challenge, which was solved by creating a Firestore collection to store messages while tracking user interactions within each chat. Thanks to Firebase integration, the application efficiently handled authentication and data storage, enabling **rapid development without the need to build a database from scratch**.