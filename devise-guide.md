# Devise Guide

This guide is only provided as a reference. Please follow the official [Devise Documentation](https://github.com/plataformatec/devise#getting-started) for an up to dat guide.

## Steps

1. Create new app

	  `$ rails new prometheus -d=postgresql`

2. Then `cd` into `prometheus`, create database inside Rails 

	  ```rails db:create```

3. Add the following line to your Gemfile file

    ```gem 'devise' ```

4. In the Terminal 

    ```bundle install```

5. Next, you need to run the generator: 

    ```rails g devise:install ```

6. Inside the `config/environments/development.rb` insert this line

    ```config.action_mailer.default_url_options = { host: 'localhost', port: 3000 }```

7. Ensure you have defined `root_url` to *something* in your `config/routes.rb`

    ```root to: 'pages#home'```

8. Make new Controller called Pages `pages_controller.rb` with method called `home`

9. Make a new folder called `pages` inside the `views` folder and create a file called `home.html.erb`

10. Inside the views layout folder, add these lines in the file `application.html.erb` file

  ```
  <p class="notice"><%= notice %></p>
  <p class="alert"><%= alert %></p> 
  ```

11. Then run `rails g devise:views` in the Terminal to make view pages for devise. For example: sign-up, sign-in, and etc.

12. `rails generate devise <Name of Model>` to create model called `User`

    ``` rails g devise User ```

13. Then run

    ``` rails db:migrate```

14. Restart the server

    To see all routes of App in Browser

    ```localhost:3000/rails/info/routes```
