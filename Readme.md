# Cron Service

## Youtube

[How To Schedule Python Scripts As Cron Jobs With Crontab](https://www.youtube.com/watch?v=5bTkiV_Aadc)

## crontab guru docs

[crontab guru](https://crontab.guru/)

command:
    ```
    crontab
    ```

options:
- -e  -- edit current crontab
- -i  -- prompt for confirmation (with - -r)
- -l  -- display current crontab
- -r  -- remove current crontab
- -u  -- specify user whose crontab to work with


examples:
- Run every 6h
    - ``` 0 0,6,12,18 * * * [command]```
- Run minute
    - ``` * * * * * [command]```

file example:
```
* * * * * python3 ~/Repositories/Github/cron-service/cron_jobs/test.py
* * * * * ~/Repositories/Github/cron-service/cron_env/bin/python3 ~/Repositories/Github/cron-service/cron_jobs/fetch_github.py

```