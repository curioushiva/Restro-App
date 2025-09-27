# 🍴 RESTRO

This repository contains the code for **RESTRO**, a complete food delivery web application built with **React, Parcel, Redux Toolkit, and custom CSS**. Designed with modular architecture and modern development practices, it provides a smooth end-to-end experience — from location-based restaurant discovery to placing and tracking food orders.

<hr style="height:3px; border:none; background-color:#3D444D;">

## ✨ Features

- **IP-based Location Detection** — Fetches user’s approximate latitude and longitude via IPinfo API to show nearby restaurants on startup
- **Place Search Integration** — Lets users search for specific locations, fetches precise lat/lng, and updates results dynamically
- **Restaurant Discovery** — Displays restaurants by city/area with clean UI and responsive design
- **Dynamic Menus** — Click any restaurant to explore categorized menus with support for multiple items and quantities
- **Cart Management** — Add/remove items, view detailed order summary with delivery charges and totals
- **User Accounts** — Sign up, log in, and manage profile details with persistent address setup (auto-fills secondary address from location)
- **Checkout & Orders** — Place orders, view delivery time/status, and download detailed bills
- **Order History** — Retains past orders, addresses, and account details (until page refresh)
- **About Page** — Showcases developer info pulled directly from GitHub, including RESTRO’s repo data
- **Shimmer UI** — Clean skeleton loaders for seamless data fetching and better UX

<hr style="height:3px; border:none; background-color:#3D444D;">

## ⚙️ Tech Stack

- **Frontend:** React, Parcel, Redux Toolkit, Custom Hooks, Custom CSS
- **State Management:** Redux Toolkit (RTK)
- **API Handling:** Fetch API (with CORS proxy)
- **UI/UX:** Shimmer UI, Responsive Design, Skeleton Loaders
- **Utilities:** IPinfo API (for geolocation), GitHub API (for About page)

<hr style="height:3px; border:none; background-color:#3D444D;">

## 🧩 Prerequisites

- [Node.js](https://nodejs.org/) (v16 or later recommended)
- npm or yarn package manager
- Git

## 🛠️ Installation & Setup

1. **Clone the repository**

   ```js
   git clone https://github.com/curioushiva/Restro.git
   cd Restro-App
   ```

2. **Install dependencies**

   ```js
   npm install
   ```

3. **Configure IPinfo API key**

   **Preferred (with API key) :**

- Go to : `Restro > src > hooks > reshook > line 35`
- Replace the fetch request with your own API key:
  ```js
  const data = await fetch(`${IpinfoFetch}${IpinfoAPIKey}`);
  ```
- This enables tracking of how many times location data is fetched, giving insights into app usage.

  **Alternative (without API key) :**

- If you don’t want to set an API key, simply remove `${IpinfoAPIKey}` from the same line:
  ```js
  const data = await fetch(`${IpinfoFetch}`);
  ```
- The app will still function, but you won’t be able to track usage statistics.

4. **Start the development server**

   ```js
   npm run start
   ```

5. **Build for production**  

   ```js
   npm run build
   ```

<hr style="height:3px; border:none; background-color:#3D444D;">

## 📦 Restro Server  

To set up your own backend server for handling API requests, please check out the companion repository here : [Restro Server](https://github.com/curioushiva/Restro-Server)  

<hr style="height:3px; border:none; background-color:#3D444D;">

## 🌐 Working Website  

You can access **[RESTRO](https://restro.curioushiva.in/)** live from here 🚀 

<hr style="height:3px; border:none; background-color:#3D444D;">

## 🤝 Contribution  

Contributions are welcome!  

1. Fork this repo  
2. Create a new branch: `git checkout -b feature-name`  
3. Commit your changes: `git commit -m "Add new feature"`  
4. Push to the branch: `git push origin feature-name`  
5. Open a Pull Request  

<hr style="height:3px; border:none; background-color:#3D444D;">

## 💡 Acknowledgments  

I have learned React from **Namaste React** by **Mr. Akshay Saini**, and his teaching played a huge role in helping me build something like RESTRO. A special thank you to him for making learning fun and practical  

<hr style="height:3px; border:none; background-color:#3D444D;">

## 👨‍💻 About the Author  

Developed with ❤️ by **[Curioushiva](https://www.instagram.com/curioushiva/)**  — Passionate in MERN development and real-world app building.  

<hr style="height:3px; border:none; background-color:#3D444D;">

## 👾 Thank You  

Thanks for checking out RESTRO!  
If you liked this project, please ⭐ the repo and share your feedback 🙌  
