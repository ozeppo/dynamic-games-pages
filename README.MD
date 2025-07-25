# 🎮 Dynamic Game Pages

**Dynamic Game Pages** is a WordPress plugin that automatically generates game subpages based on live Steam API data — perfect for SEO, game directories, affiliate sites, and more.

---

## ✨ Features

* Fetches real-time game data from Steam (title, description, price, requirements, etc.)
* Creates SEO-friendly URLs like `/game/{appid}`
* Customizable shortcode banner: `[game_banner appid="123456"]`
* Editable color theme and FAQ text
* Supports multiple languages (based on Steam data availability)
* Outputs Schema.org FAQ & VideoGame JSON-LD for rich search results
* Native Gutenberg block to insert banners without using shortcodes
* Elementor widget for drag-and-drop banner integration

![Dynamic ganerated game page](https://i.imgur.com/9TVUf9B.png)

---

## 📦 Installation

1. Download or clone the plugin:

   ```bash
   git clone https://github.com/ozeppo/dynamic-games-pages.git
   ```
2. Copy the folder into your WordPress `/wp-content/plugins/` directory
3. Go to **Plugins > Installed Plugins** in WordPress and activate "Dynamic Game Pages"
4. Navigate to **Settings > Dynamic Game Pages** to configure

---

## ⚙️ Configuration

Available settings:

* **Game Slug** – base slug for game pages (e.g. `/game/1091500`)
* **Accent Color** – used in buttons and section headers
* **Steam Language** – language used in API requests (`english`, `polish`, `german`, etc.)
* **FAQ Templates** – dynamic text placeholders:

  * `%title` – game name
  * `%release` – release date
  * `%requirements` – system requirements

> ⚠️ After changing the slug, go to **Settings > Permalinks** and click “Save Changes” to refresh rewrite rules.

---

## 🧹 Shortcode & Block Support

Use this shortcode anywhere in your site:

![Dynamic ganerated game banner with Steam price](https://i.imgur.com/hWchnoa.png)

```php
[game_banner appid="1091500" button="Buy on Steam"]
```

### Gutenberg & Elementor support

This plugin also includes:
- A Gutenberg block called “Game Banner” you can insert directly into posts/pages
- An Elementor widget for visual page building

Both options work the same way as the shortcode and use the same output logic.

---

## 🔍 Example Output

Generated game page includes:

* Game title & header image
* Description, release date, genre
* Publisher & developer info
* Price (converted via Steam API)
* System requirements (minimum & recommended)
* FAQ section with structured JSON-LD

---

## 🌐 Translations

* Fully gettext-compatible (`__()`, `_e()`, etc.)
* Translation-ready via `.pot` file in `/languages/`
* Works great with Loco Translate or WPML

---

## 💪 Requirements

* WordPress 5.8 or higher
* PHP 7.4 or higher
* External HTTP access (for Steam API)

---

## 👨‍💻 Author

**Filip Chmielecki**
[filipchmielecki.pl](https://filipchmielecki.pl)
[wiemwcogram.pl](https://wiemwcogram.pl)
Plugin created to support content creators and SEO-focused game websites.

---

## 🧠 Contributions & Support

Suggestions and bug reports welcome!
Please submit issues or pull requests on [GitHub](https://github.com/ozeppo/dynamic-games-pages/issues)
