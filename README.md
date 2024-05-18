# [Flask Material Kit](https://appseed.us/product/material-kit/flask/)

`Open-Source` **[Flask App](https://appseed.us/apps/flask/)** crafted on top of a modern **Bootstrap 5** UI. Designed for those who like bold elements and beautiful websites, **Material Kit 2** is ready to help you create stunning websites and web apps. `Material Kit 2` is built with over 60 frontend individual elements, like buttons, inputs, navbars, nav tabs, cards, or alerts, giving you the freedom of choosing and combining.

- 👉 [Flask Material Kit](https://appseed.us/product/material-kit/flask/) - product page
- 👉 [Flask Material Kit](https://flask-material-kit.appseed-srv1.com/) - LIVE App

<br />

## Features

> `Have questions?` Contact **[Support](https://appseed.us/support/)** (Email & Discord) provided by **AppSeed**

| Free Version                          | [PRO Version](https://appseed.us/product/material-kit2-pro/flask/)          | [Custom Development](https://appseed.us/custom-development/) |  
| --------------------------------------| --------------------------------------| --------------------------------------|
| ✓ **Up-to-date dependencies**             | **Everything in Free**, plus:                                        | **Everything in PRO**, plus:          |
| ✓ Best Practices                          | ✅ **Premium Bootstrap 5 Design**                                    | ✅ **1 Week** `Custom Development`   |
| ✓ DB: SQLite, MySql                       | ✅ **PRO Support** - [Email & Discord](https://appseed.us/support/)  | ✅ **Team**: PM, Developer, Tester   |
| ✓ DB Tools: ORM, Flask-Migrate            | ✅ `Private REPO Access`                                             | ✅ Weekly Sprints                    |
| ✓ Session-Based authentication            |  -                                                                    | ✅ Technical SPECS                  |
| ✓ `Docker`                                |  -                                                                    | ✅ Documentation                    |
| ✓ `CI/CD` Flow via Render                 |  -                                                                    | ✅ **30 days Delivery Warranty**    |
| ✓ `Free Support`                          |  -                                                                    | ✅ [CI/CD for AWS, DO](https://appseed.us/terms/#section-ci-cd) **(Extra)**    |
| ---------------------------------         | ---------------------------------                                     | ---------------------------------  |
| ✓ [LIVE Demo](https://flask-material-kit.appseed-srv1.com)  | 🚀 [LIVE Demo](https://flask-material-kit2-enh.appseed-srv1.com) `PRO` | 🛒 `Order`: **[$999](https://appseed.gumroad.com/l/rocket-package-week)** (GUMROAD) |

![Material Kit - Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/167396765-c88b7a95-155f-4236-8691-7b80fa2d9cd9.png)

<br />

## Start with `Docker`

> 👉 **Step 1** - Download the code from the GH repository (using `GIT`) 

```bash
$ git clone https://github.com/app-generator/flask-material-kit.git
$ cd flask-material-kit
```

<br />

> 👉 **Step 2** - Start the APP in `Docker`

```bash
$ docker-compose up --build 
```

Visit `http://localhost:5085` in your browser. The app should be up & running.

<br />

## ✨ How to use it

> Download the code 

```bash
$ git clone https://github.com/app-generator/flask-material-kit.git
$ cd flask-material-kit
```

<br />

### 👉 Set Up for `Unix`, `MacOS` 

> Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Flask Environment

```bash
$ export FLASK_APP=run.py
$ export FLASK_ENV=development
```

<br />

> Start the app

```bash
$ flask run
```

At this point, the app runs at `http://127.0.0.1:5000/`. 

<br />

### 👉 Set Up for `Windows` 

> Install modules via `VENV` (windows) 

```
$ virtualenv env
$ .\env\Scripts\activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Flask Environment

```bash
$ # CMD 
$ set FLASK_APP=run.py
$ set FLASK_ENV=development
$
$ # Powershell
$ $env:FLASK_APP = ".\run.py"
$ $env:FLASK_ENV = "development"
```

<br />

> Start the app

```bash
$ flask run
```

At this point, the app runs at `http://127.0.0.1:5000/`. 

<br />

### 👉 Create Users

By default, the app redirects guest users to authenticate. In order to access the private pages, follow this set up: 

- Start the app via `flask run`
- Access the `registration` page and create a new user:
  - `http://127.0.0.1:5000/register`
- Access the `sign in` page and authenticate
  - `http://127.0.0.1:5000/login`

<br />

## ✨ `Go LIVE` via [LIVE Deployer](https://appseed.us/go-live/)

> This video explains `how to deploy` the product LIVE using a `Drag & Drop` gesture.

<br />

https://user-images.githubusercontent.com/51070104/202416162-885c30d3-5066-40cb-abcd-1668689c9463.mp4

<br />

## Codebase structure

The project is coded using blueprints, app factory pattern, dual configuration profile (development and production) and an intuitive structure presented bellow:

```bash
< PROJECT ROOT >
   |
   |-- apps/
   |    |
   |    |-- home/                           # A simple app that serve HTML files
   |    |    |-- routes.py                  # Define app routes
   |    |
   |    |-- authentication/                 # Handles auth routes (login and register)
   |    |    |-- routes.py                  # Define authentication routes  
   |    |    |-- models.py                  # Defines models  
   |    |    |-- forms.py                   # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>          # CSS files, Javascripts files
   |    |
   |    |-- templates/                      # Templates used to render pages
   |    |    |-- includes/                  # HTML chunks and components
   |    |    |    |-- navigation.html       # Top menu component
   |    |    |    |-- sidebar.html          # Sidebar component
   |    |    |    |-- footer.html           # App Footer
   |    |    |    |-- scripts.html          # Scripts common to all pages
   |    |    |
   |    |    |-- layouts/                   # Master pages
   |    |    |    |-- base-fullscreen.html  # Used by Authentication pages
   |    |    |    |-- base.html             # Used by common pages
   |    |    |
   |    |    |-- accounts/                  # Authentication pages
   |    |    |    |-- login.html            # Login page
   |    |    |    |-- register.html         # Register page
   |    |    |
   |    |    |-- home/                      # UI Kit Pages
   |    |         |-- index.html            # Index page
   |    |         |-- 404-page.html         # 404 page
   |    |         |-- *.html                # All other pages
   |    |    
   |  config.py                             # Set up the app
   |    __init__.py                         # Initialize the app
   |
   |-- requirements.txt                     # App Dependencies
   |
   |-- .env                                 # Inject Configuration via Environment
   |-- run.py                               # Start the app - WSGI gateway
   |
   |-- ************************************************************************
```

<br />

## [Flask Material Kit](https://appseed.us/product/material-kit2-pro/flask/) `PRO`

> For more components, pages and priority on support, feel free to take a look at this amazing starter:

**Material Kit 2** is a premium design crafted by the `Creative-Tim` agency on top of Bootstrap 5 Framework. Designed for those who like bold elements and beautiful websites, Material Kit 2 is made of hundreds of elements, designed blocks, and fully coded pages built with an impressive level of quality.

- 👉 [Flask Material Kit2 PRO](https://appseed.us/product/material-kit2-pro/flask/) - product page
  - ✅ `Enhanced UI` - more pages and components
  - ✅ `Priority` on support

<br >

![Mk2 PRO - Premium Seed project by AppSeed.](https://user-images.githubusercontent.com/51070104/168224733-b054bb46-d454-4aea-bb94-2d01bf4760d2.png)

<br />

---
[Flask Material Kit](https://appseed.us/product/material-kit/flask/) - Open-source starter generated by **[App Generator](https://appseed.us/generator/)**.
