# Bubble Shop

[![中文文档](https://img.shields.io/badge/文档-中文-blue?style=flat-square)](README_ZH.md)

An e-commerce project built with **Jetpack Compose**, paired with a self-hosted backend, demonstrating end-to-end implementation for mobile and server sides.

## 🧱 Tech Stack

### 🤖 Android

| Module                           | Description                                                                                           |
|:---------------------------------|-------------------------------------------------------------------------------------------------------|
| UI                               | Jetpack Compose                                                                                       |
| Network                          | Retrofit + OkHttp                                                                                     |
| DI                               | Hilt                                                                                                  |
| Architecture                     | Layered architecture with module decoupling, focused on reusability, testability, and maintainability |
| State Management                 | Isolated events and states across modules to ensure separation of business logic and UI               |
| Lightweight Global Dependencies  | Global dependency management module for providing shared resources and common services                |

### ☕ Backend

| Module         | Technology                                               |
|:---------------|----------------------------------------------------------|
| Framework      | Spring Boot + JPA                                        |
| Authentication | JWT                                                      |
| Database       | MySQL(self-hosted, local deployment)                     |
| API            | RESTful APIs providing product, user, cart data services |

## 🎯 Development Goals

To validate the maintainability and scalability of Compose architecture in mid-to-large scale projects, and explore full-stack mobile-server workflows and performance boundaries.

The focus is **on in-depth Android technical practice**, rather than complete business functionality.

## 🧩 Features

* Authentication
    * Login and logout
    * Route interception
* Home screen product feed
  * lazy-loaded waterfall layout
  * **Pagination** Loading Data
* Product detail screen
    * Immersive gradient toolbar on scroll
    * Infinite carousel for product banners
    * Full-screen preview on banner click
    * Add to cart support
* Cart module (display)
* Permissions handling
* User profile screen
    * Theme mode switching

## 📱 Screenshot Preview

|           Screen           |                                 Screenshot                                  |
|:--------------------------:|:---------------------------------------------------------------------------:|
|       Splash Screen        |        <img src="screenshots/splash.png" alt="Splash" height="500"/>        |
| Login + Route Interception |         <img src="screenshots/login.gif" alt="Login" height="500"/>         |
|        Home Screen         |          <img src="screenshots/home.gif" alt="Home" height="500"/>          |
|       Product Detail       |    <img src="screenshots/product_detail.gif" alt="Detail" height="500"/>    |
|        Add to Cart         |  <img src="screenshots/add_cart_item.gif" alt="AddCartItem" height="500"/>  |
|   Cart Display & Update    |          <img src="screenshots/cart.gif" alt="Cart" height="500"/>          |
|       Profile Screen       |            <img src="screenshots/me.png" alt="Me" height="500"/>            |
|      Photo Permission      |    <img src="screenshots/permission.gif" alt="Permission" height="500"/>    |
|     Failed Photo Fetch     | <img src="screenshots/fail_get_image.gif" alt="FailGetImage" height="500"/> |
|      Theme Switching       |         <img src="screenshots/theme.gif" alt="Theme" height="500"/>         |
|           Logout           |        <img src="screenshots/logout.gif" alt="Logout" height="500"/>        |

## 🚧 Planned Features

* Product search
* Cart module (quantity modification)
* User profile screen (avatar cropping)
