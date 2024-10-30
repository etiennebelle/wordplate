# Wordplate Starter ⚡️

## Installation

- **Wordpress + Composer**

`composer update`

## Features

- **Vite JS** For building and minifying your CSS and JavaScript

```
# Start the dev server...
npm run dev

# Build for production...
npm run build
```

- **Sass**

## Theme

You can rename the theme directory and modify `.env`
```
WP_DEFAULT_THEME=theme
```

## Configuration

### Public Dir

After installing WordPlate, you'll need to configure your web server's document or web root to be the `public` directory. This is where the main entry point for your application, `index.php`, is located.

`.htaccess`
```
RewriteEngine On
RewriteCond %{HTTP_HOST} ^[subdomain]\.domain\.fr$ [NC,OR]
RewriteCond %{HTTP_HOST} ^www\.[subdomain]\.domain\.fr$ [NC]
RewriteCond %{REQUEST_URI} !^/public/
RewriteRule ^(.*)$ /public/$1 [L]
```

### Environment Configuration

- **Environment Files**

`.env`
```
DB_NAME=database
DB_USER=username
DB_PASSWORD=password
```


### Salt Keys

Visit the generator (**https://vinkla.github.io/salts/**) and copy the randomly generated keys to your `.env` file.

```
AUTH_KEY=
SECURE_AUTH_KEY=
LOGGED_IN_KEY=
NONCE_KEY=
AUTH_SALT=
SECURE_AUTH_SALT=
LOGGED_IN_SALT=
NONCE_SALT=
```
