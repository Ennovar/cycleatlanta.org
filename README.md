# cycleatlanta.org
The cycleatlanta.org is a set of web applications. It's primary function is to collect, organize and publish bike path data from bicyclists.

* [cycleatlanta.org/index.html](cycleatlanta.org) - A static web page shows detailed information about Cycle Atlanta. 
* Post back-end webapp - A web application to collect bike path data from bicyclists' mobile applications. This application is compatible with Cycle Tracks based mobile applications:
	* [Cycle Atlanta Android](https://github.com/CUTR-at-USF/Cycle-Atlanta-Android)
	* [Cycle Atlanta iOS](https://github.com/CUTR-at-USF/Cycle-Atlanta-iOS)
	* [Cycle Tracks](https://github.com/sfcta/CycleTracks)
* Rides webapp - A user interface to see bike path data from bicyclists.

## Getting Started

Here are the high-level steps you'll need to take to launch the cycleatlanta.org back-end webapps.

1. Create a MySql database and generate tables by running the [cyleatlanta sql script](https://github.com/cagryInside/cycleatlanta.org/tree/master/database).
2. Use a PHP and http server (e.g., [WAMP](http://www.wampserver.com/en/), [XAMPP](https://www.apachefriends.org/index.html))
3. Copy `cycleatlanta.org` and `include` folders to web server's `www` folder
4. Organize the imports in the `/post_dev/index.php` file based on the 'include' folders' location. You might need to use full path if you are using windows.
5. For the Rides web app, organize the imports in the `rides/getData.php`
6. Set your database credentials into `include/Database_dev.php`
7. Restart the server
8. The post url should be `localhost:port/post_dev/index.php`
9. The information web page's url should be `localhost:port/index.html`
10. The Rides webapp's url shoud be `localhost:port/rides/index.php`




