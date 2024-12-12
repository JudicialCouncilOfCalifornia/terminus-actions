# Using Github Actions to Schedule Drush Commands

These workflows are scheduled drush commands sent to Pantheon via Terminus.

## Cron Scheduling
Github is on UTC time so you have to adjust to PST. For example, 14 UTC is 6:00 AM DST or 7:00 AM.

Jobs will not necessarily run at expected time so you may need to adjust the timing to gain relative accuracy.
For example, Granicus event imports are set to run 15 minutes prior to the hour but the job actually runs 3-5 minutes
before or after the hour.

## Migrate Command Arguments
[Drush Documentation](https://www.drush.org/13.x/commands/migrate_import/)
