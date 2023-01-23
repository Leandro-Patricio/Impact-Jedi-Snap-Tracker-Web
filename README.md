# Impact-Jedi-Snap-Tracker-Web

This project was created to fulfill the Impact Jedi challenge. 

Although what's here wasn't exactly what they asked for, I took the opportunity to do a personal project, a manual deck tracker for the Marvel Snap card game. This project is still under construction, as I want to expand the project so that it can be online and share it with friends and interested parties.

To access the figma of this project, click [here](https://www.figma.com/file/NOjngJpxF8a6MlfJFpuoeZ/Snap-manual-deck-tracker?node-id=6%3A11&t=9lQBFtWzcmzQEsGm-0).

I used the marvelSnapPro website API to access the card information, https://static2.marvelsnap.pro/snap/do.php?cmd=getcards, and the images, https://static.marvelsnap.pro/cards /Abomination_03.webp

All requirements have been met for this challenge

The project in this repository represents the frontend of my project. I strongly recommend using it with the backend, which is [in this repository](https://github.com/Leandro-Patricio/Impact-Jedi-Snap-Tracker-Server).

For more detailed information on the process, 
[visit access your repository](https://github.com/Impact-Plataform/Banco-de-talentos/tree/main/frontend)

## Table of contents

* [Technologies](#technologies)
* [Installation](#Installation)
* [Usage](#usage)

## Technologies

Project is created with:
* Front-end

1. ![Image](https://img.shields.io/badge/Next.js-13.1.1-yellowgreen)
2. ![Image](https://img.shields.io/badge/Typescript-4.9.4-blue)
3. ![Image](https://img.shields.io/badge/React-18.2.0-orange)
4. ![Image](https://img.shields.io/badge/TailwindCSS-3.2.4-green)
5. ![Image](https://img.shields.io/badge/Axios-1.2.2-lightgrey)
---


## Installation

After cloning

```bash
npm i
npm run dev
```
This project has not yet been deployed. I intend to do it with vercel


## Usage

First you will see tha landing page, with the option register and login.

![landing page](https://i.postimg.cc/tCskCR2h/landingpage.png)

To login, you will need first to register an account. Clicking on register, an modal will show up. Your username has to be unique and your password has to follow some rules.

![register modal](https://i.postimg.cc/bvx3c6LW/cadastro.png)

---

Once logged in, you will be redirected to the home page (My account), and you will be able to browse 4 pages: Collection, All cards, Play and Friends.

![home](https://i.postimg.cc/G37zCTJL/myaccount.png)

The Play and Friends pages are still under construction, so they don't have implemented features

On the All cards page, you will have access to the cards registered so far by MarvelSnapPro. You can filter cards by name, cost, power, pool, and skill. In addition, the letters are paginated.

When you click on a card on this page, you will be redirected to that card's page, where you will find more information about it, in addition to images of its variant arts.

Note that when hovering, you will see the letter a little larger with more information.

![solitary cards](https://i.postimg.cc/wMvVN9HY/solitarycard.png)

---
On the Collection page, you can also see the same cards as on the All Cards page, also with filters and pagination. However, the difference is in its main functionality. When clicking on a card, it will change from black and white to color. Under the covers, when the card turns color, it is being added to your collection in the database (and removed when it turns black and white). This information is saved for when you log in again.

In addition to helping you know which cards you still don't have, although not yet implemented, when you can assemble your decks, only the cards in your collection will be available.

![my collection](https://i.postimg.cc/8c0bBxPJ/mycollection.png)

It should be noted that all pages are fully responsive, even for the smallest of cell phones

![responsive](https://i.postimg.cc/76qXxgW6/responsive.png)

---
Yes, you have the option to log out. As soon as you log out, your jwt token is cleared from memory and you can log in with another valid username and password.

![logout](https://i.postimg.cc/NMbDL53x/logout.png)

