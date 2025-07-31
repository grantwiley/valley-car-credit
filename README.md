# Valley Car Credit Website (Eleventy Version)

A fully responsive, accessible static website for Valley Car Credit, rebuilt with the Eleventy static site generator.

## 🚀 Quick Start

This project is now powered by Eleventy, a simpler static site generator.

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/grantwiley/valley-car-credit.git
    cd valley-car-credit
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

### Development

To start the local development server with hot reloading:

```bash
npm start
```

This will open a local server, typically at `http://localhost:8080`. The site will automatically reload when you make changes to the source files.

### Build for Production

To build the static site for production:

```bash
npm run build
```

The generated files will be in the `dist` directory.

### Deployment to Sevalla

1.  **Run the build command:**
    ```bash
    npm run build
    ```
2.  **Upload the `dist` directory** to your Sevalla hosting service.
3.  **Configure your hosting** to serve the site from the `dist` directory.

## 📁 File Structure

```
valley-car-credit/
├── src/
│   ├── _includes/          # Reusable components (partials)
│   ├── _layouts/
│   │   └── base.njk        # Main layout template
│   ├── blog/               # Blog posts
│   ├── contact/
│   │   └── index.html      # Contact page
│   ├── css/
│   │   └── styles.css
│   ├── images/
│   │   └── vcc-logo.jpg
│   ├── js/
│   │   └── main.js
│   ├── credit-improvement/
│   │   └── index.html
│   ├── make-payment/
│   │   └── index.html
│   ├── online-account/
│   │   └── index.html
│   ├── resources/
│   │   └── index.html
│   ├── index.html          # Homepage
│   └── favicon.ico
├── .eleventy.js            # Eleventy configuration
├── package.json
└── README.md
```

## 🎨 Customization

### Colors and Branding

-   Edit `src/css/styles.css` to change colors, fonts, etc.

### Content

-   **Pages**: Edit the HTML files in their respective folders (e.g., `src/contact/index.html`).
-   **Blog Posts**: Add new folders and `index.html` files to `src/blog/`.

### Navigation

-   The navigation menu is managed in `src/_layouts/base.njk`.

## ✨ Key Features

-   **Static Site Generation**: Fast, secure, and easy to deploy.
-   **Clean URLs**: Pages are available at `/contact/` instead of `/contact.html`.
-   **Maintainable**: Reusable layouts and a centralized structure make updates easier.
-   **Responsive & Accessible**: Mobile-first and built with accessibility best practices.
-   **SEO Optimized**: Structured data, meta tags, and semantic HTML.
