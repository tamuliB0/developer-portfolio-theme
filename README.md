# Developer Portfolio Theme

### A clean, fast WordPress portfolio theme built from scratch using classic PHP templates.

This theme is a personal portfolio made for web developers. It's built without page builders or heavy starter themes — just clean code, WordPress core functions, and a proper template structure.


## 🚀 Features

- **Classic Template Structure:** Uses standard WordPress files like `header.php`, `footer.php`, `index.php`, `single.php`, and `functions.php`
- **Custom Navigation:** Menus you can manage directly from the WordPress admin panel
- **Mobile-First Design:** Responsive CSS built for fast load times on all screen sizes
- **Widget Support:** Sidebar and footer areas ready for WordPress widgets
- **Plugin-Ready:** Uses `wp_head()` and `wp_footer()` hooks so plugins work out of the box


## 🛠️ Built With

- **CMS:** WordPress 7.0
- **Language:** PHP 8.3.6
- **Local Environment:** DDEV 1.25.2


## 📋 Prerequisites

To run this application locally, your system must have Docker and DDEV installed. Follow the links below for easy, step-by-step setup guides depending on your operating system:

1. **Docker CE / Container Engine**
   - Linux Users: [Official Docker Installation Guide for Linux](https://docs.docker.com/engine/install/)
   - Mac/Windows Users: [Docker Desktop Installation Guide](https://docs.docker.com/desktop/)
2. **DDEV CLI**
   - Follow the [Official DDEV Installation Script & Guide](https://ddev.readthedocs.io/en/stable/users/install/ddev-installation/) for all platforms.


## ⚙️ Setup Instructions

### 1. Create a Local WordPress Site with DDEV

If you don't have a local WordPress project yet, run these commands:

```bash
mkdir developer-portfolio-theme && cd developer-portfolio-theme
ddev config --project-type=wordpress
ddev start
ddev wp core download
ddev wp core install --url='$DDEV_PRIMARY_URL' --title="YOUR-WEBSITE-TITLE" --admin_user=admin --admin_password=admin --admin_email=admin@example.com
```
Your site will be at `https://<your-ddev-project-name>.ddev.site`. Admin login: `admin` / `admin`.

### 2. Clone the Theme

Go to your WordPress themes folder and clone this repo:

```bash
cd wp-content/themes
git clone https://github.com/tamuliB0/developer-portfolio-theme.git
```

### 3. Activate the Theme

1. Run `ddev launch` to open your site in the browser
2. Log in to the WordPress dashboard at `/wp-admin`
3. Go to **Appearance > Themes**
4. Find **Developer Portfolio Theme** and click **Activate**


## 💻 Usage

### 🏠 Local Development

Your local site runs at: `https://<your-ddev-project-name>.ddev.site`

### 🌐 Live Demo

👉 [View Live Site](http://www.bhardwaj.lovestoblog.com/wp/)

---

### 🛠️ Useful Commands

- `ddev start` — Starts your local WordPress site and database
- `ddev stop` — Stops the project without losing any data
- `ddev describe` — Shows your local URLs and database credentials
