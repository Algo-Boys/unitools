# Tools/config for University of Tübingen

## Config

-   eduroam for iwd: Move `eduroam.8021x` to `/var/lib/iwd/`. Move the
    public certificate `eduroam.crt` to `/opt/eduroam.crt`. Don't forget
    to assign the correct permissions.

## Scripts

-   `almanot`: Get notifications if something on Alma changes. Uses the
    official RSS feed endpoint.
-   `iliasnot`: Get notifications for changes of course pages.
    *UNOFFICIAL* scraping method, only use this script if you have
    permission to scrape the website!

Then `crontab -e` and `*/10 * * * * <PATH>/almanot` to check every 10
minutes.
