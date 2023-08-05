<p align="center" width="100%">
    <img width="20%" src="./profile/logo.svg"> 
</p>

# Svelte SE

Svelte SE is a collection of tools and startup packages designed for the SvelteKit framework, aiming to streamline development. Our mission is to make the development process enjoyable and innovative, empowering developers to create robust and scalable applications with ease. Sveltes SE simplifies common tasks and enhances the SvelteKit experience by offering:

- Pre-configured, modular starter templates.
- Efficient state management solutions.
- Out-of-the-box integrations with popular backend services.
- Comprehensive UI component libraries. (coming soon)

Sveltese is user-friendly, adaptable, and equips developers with the resources needed to build and maintain large-scale applications.

## Installation

```
npm create sveltese@latest app_name
```
If you are already familiar with SvelteKit you will recognize the CLI.

```
create-svelte version 0.0.2

┌  Welcome to SvelteKit!
│
◆  Is this a SvelteKit SE project?
│  ● Yes / ○ No
└
```

```
npm install
```

NPM install will magically make a new .env file in your root directory.  It is copying .env.example.  Inside .env there is a database url that is setup for postgresql.  You will need to create a database named sveltese and a user named sveltese with no password.  Or you will need to modify the DATABASE_URL string to fit your connection and credentials.

```
npm db:init
```
This will get prisma running.  It will create a migration table, setup the tables needed for lucia auth and create zod models to validate against.

This will also create a test user.

```
npm dev
```

That's all there is to it.  You can build your next great idea with a solid authentication system prebuilt in sveltekit.  p



## The Future

For now we are using TailwindCSS for styles.  This allows for MeltUI, DaisyUI, SkeletonUI and all the others.  There is no clear UI winner yet. \

The dashboard is where you can go with the Logged in state.  All you can do there.. is logout and there is no UI.  I'm thinking to add a user profile section there so people can upload avatars or change their email and so on.  

As for database, I am working on on sqlite first.  It would make the starter easier without having to know psql and run it locally.

Docs would be nice, but this will have to do for now.  

Github Login, Google Login, LinkedIn Login, Facebook Login, Twitter Login, likely in that order.   

Drop me a note if you have any good ideas. 

Throw me some code if your really feeling it.  :)




## Authentication

Svelte SE uses is using Prisma, Lucia and Postgres, as well as nodemailer and mailpit, to create a drop in authentication system.

