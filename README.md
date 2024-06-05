These are the scripts to clear the browser cache in linux. The files are respectively for brave browser, google chrome, fiefox and linux mint webapps. If you want these scripts to run automatically copy these files to one of the cron directories.

Steps to automatically run these scripts every hour:
1. Download the required file according to the browser that you are using.
2. Make it executable
     chmod +x clear_brave_cache
     chmod +x clear_chrome_cache
     chmod +x clear_firefox_cache
     chmod +x clear_webapp_manager_cache
3. Change the owner of the file to root
     sudo chown root:root clear_brave_cache
     sudo chown root:root clear_chrome_cache
     sudo chown root:root clear_firefox_cache
     sudo chown root:root clear_webapp_manager_cache
4. Move the files to /etc/cron.daily
     sudo mv clear_brave_cache /etc/cron.daily/
     sudo mv clear_chrome_cache /etc/cron.daily/
     sudo mv clear_firefox_cache /etc/cron.daily/
     sudo mv clear_webapp_manager_cache /etc/cron.daily/

Now the script will automatically run every hour. This will prevent the browser cache from using up your disk space.
