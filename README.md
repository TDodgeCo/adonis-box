## Adonis-Box

Adonis-Box is a no frills vagrant box built specifically for running AdonisJS applications on Ubuntu 16.04.
Designed from the start with simplicity in mind. No complicated setup required.
Simply clone this repo and run `vagrant up` and you're pretty much ready to start coding.

### Get Started

1) Clone this repo and `cd` into it's new directory

2) Run `vagrant up`

3) Run `vagrant ssh`

4) Run `cd /var/www/ && adonis new <your application name>`

5) Run `nodemon server.js` and open `http://192.168.33.10/` in your browser

There should now be a new folder in your local machine's root directory with your applications name. Open that in your favorite text editor and get to coding!

**OPTIONAL** - If you have an existing AdonisJS project that you would like to run inside Adonis-Box, simply clone it into `/var/www`. You'll need to make sure that you create a new `.env` file with an application key, otherwise it won't run.

### What's Included

1) Ubuntu 16.04

2) Node 8.11.2

3) NPM 5.6.0

4) Adonis-CLI 4.0.5

5) MySQL 5.7.22

6) Redis 4.0.9

7) Nodemon 1.17.5

8) PM2 2.10.4

### Access Info

#### MySQL
Database: `adonis`

User: `root`

Password: `root`

Port: `3306`

While SSH'd into the box, type `mysql -u root -p`. You'll be prompted for the password.

**IMPORTANT:** 
You will still need to install the MySQL providers for adonis. Once you've done that, Adonis-Box is configured to work with the standard environment variables found in your `.env` file.  You'll just need to change the database to `MySQL`.

#### Redis

Port: `6379`

**IMPORTANT:** 
You will steel need to install the Redis providers for Adonis. Once you've done that, Adonis-Box is configured to work with Redis right away.

### Coming Soon

Postgres support

