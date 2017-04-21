# Getting started with Web Development using WordPress

## Setting up you local environment

### Pre-requisites

#### 1) XAMP
Used to have a local development environment
https://www.apachefriends.org/download.html

* Apache (server)
* MySQL (database)
* PHP (language)

#### 2) WordPress files
https://wordpress.org/download/ (latest 4.7.4)
* extract to your localhost folder in a subfolder of your name

or 

* git clone https://github.com/WordPress/WordPress.git

or

* bower install wordpress

or

* npm install wordpress

  package.json
    var wordpress = require( "wordpress" );
    var client = wordpress.createClient({
      url: "my-site.com",
      username: "admin",
      password: "secret"
    });
 
    client.getPosts(function( error, posts ) {
        console.log( "Found " + posts.length + " posts!" );
    });
    
or 

* wp cli > wp install



#### 3) Setup database
mysql -uroot -p1234 -e "CREATE DATABASE 'db_name';
mysql -uroot -p1234 -e "CREATE USER db_name@localhost IDENTIFIED BY 1234;"
mysql -uroot -p1234 -e "GRANT ALL PRIVILEGES ON db_name.* TO 'db_user'@'localhost';"
mysql -uroot -p1234 -e "FLUSH PRIVILEGES;"
* Sample is for demo usage only, do not use this for live

### 4) Installation
run your localhost
http://localhost/yourname
mine
http://localhost/test/wp1

##### Put in all parameters needed
- DB creds
- Site name
- Email
- admin username
- admin pass

## Things to do after installing WordPress

### 1) Get a theme

Edit theme
Appearance > customize
- Theme title & description
- Add logo
- Change background image / color
- Customize header and footer

### 2) Plan your pages
1. Homepage
2. About pages
3. Blog pages
4. Contact me pages

### 3) Setup your menu structure and position

## Extending your self-hosted WordPress

### 1) Install a plugin
What are plugins?
https://wordpress.org/plugins/jetpack/

### 2) Create a blog post

### 3) custom widgets


### Deployment to live
