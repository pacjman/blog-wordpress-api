## blog-wordpress-api 

> Look, I made this for you.<br/>
> ... How can you use this already?<br/>

### Setup

* Clone the latest sources from [GitHub](https://github.com/).

``` bash
git clone https://github.com/pacjman/blog-wordpress-api
```

* Install those dependencies.

``` bash
npm install
```

* Copy the provided `.env-dist` file to `.env`, like so:

``` bash
cp .env-dist .env
```

* Modify the `.env` file to match your Wordpress DB settings. Provide values where the helpful mustaches suggest.

``` javascript
WORDPRESS_DB_HOST={{host}}
WORDPRESS_DB_USER={{user}}
WORDPRESS_DB_PASSWORD={{password}}
WORDPRESS_DB_NAME={{name}}
```

> For example, let's pretend you have a local [MySql](https://mysql.com/) instance ready. Then modify as follows:

``` javascript
WORDPRESS_DB_HOST=localhost
WORDPRESS_DB_USER=user
WORDPRESS_DB_PASSWORD=superSecretPassword
WORDPRESS_DB_NAME=wordpress
```

> Don't forget to adjust these fields to match your configuration.

### Build 

* Build it.

``` bash
npm run build
```

### Start

* Light it up!

``` bash
npm run start
```

### Conclusion

* So that's really it. Now you have a simple, read-only api wrapping the heart of ~~darkness~~ [Wordpress](https://wordpress.org/). Yay!

### Other

* There's a [Postman](https://www.getpostman.com/) collection & env saved to prove functions [here](https://github.com/pacjman/blog-wordpress-api/tree/master/tests/postman).

### References

* [Developing a Restful Api w/ Node & TypeScript](https://mherman.org/blog/2016/11/05/developing-a-restful-api-with-node-and-typescript/)
* [Express routing](https://expressjs.com/en/guide/routing.html)
* [Get Postman for API development](https://www.getpostman.com/apps)
