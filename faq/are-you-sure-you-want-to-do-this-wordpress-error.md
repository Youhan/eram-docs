# Are you sure you want to do this? WordPress Error

This is not a theme issue or bug.

If you are installing Eram theme from the WordPress theme installer, but get a message that says _**Are you sure you want to do this?**_, most likely your web server is configured with a PHP settings that only allow a certain size ZIP file to be uploaded via WP admin.

Most hosting companies configure their servers to only have the maximum file upload size limit at 8-10 MB, some are less. Eram theme zip file is around 14mb because of available plugins and all demos and WordPress is unfortunately giving you a rather ambiguous message in response.

**There two ways to solve this problem.**

* You can get your web host to increase your PHP limits so a larger zip file is allowed to be uploaded. They will know which limits to set if you explain the issue. Here are some recommended configurations:
  * max\_execution\_time 60
  * memory\_limit 128M
  * post\_max\_size 48M
  * upload\_max\_filesize 48M
* You can unzip theme zip file and upload the content directly to WordPress -

  &gt;

   wp-content-

  &gt;

  themes  theme via FTP and then go to dashboard-

  &gt;

  appearance-

  &gt;

  themes and activate Eram.

