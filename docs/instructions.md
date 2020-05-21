```sh
rails new applocale_dev
cd applocale_dev
```

```
➜ rails app:template LOCATION="https://railsbytes.com/script/X8Bsjj"
         run  spring stop from "."
Spring is not running
👋 Welcome to AppLocale's installation process

ℹ️   You'll need to open up https://applocale.dev in your browser.
     - Login
     - Click the avatar and open the dropdown
     - Click API Tokens
     - Create a new API Token

ℹ️  If you don't yet have a project, make sure you create one and setup your languages first!

🙌 Okay next up we'll ask for the API Token, and Project ID which you can find on the API Tokens page.

What is your AppLocale API Token? xxxxx
What is your Project ID? xxxxx
```

remove

RailsBytes: dotenv-rails
```sh
rails app:template LOCATION='https://railsbytes.com/script/zOvsQ0'
```

Setup
```sh
rails app:template LOCATION='https://railsbytes.com/script/xYas74'
```

Pull down translations
```sh
➜ bundle exec applocale pull
[AppLocale] Fetching list of languages...
[AppLocale] Fetching translations for en...
[AppLocale] ↳ Wrote translations for en to config/locales/en.yml
[AppLocale] Fetching translations for es...
[AppLocale] ↳ Wrote translations for es to config/locales/es.yml
```

```sh
➜ ls config/locales
en.yml es.yml
```

<%= t("home.welcome") %>

rails s

http://localhost:3000/home/index?locale=en
http://localhost:3000/home/index?locale=es
