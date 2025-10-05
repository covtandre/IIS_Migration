# IIS_Migration
<img width="910" height="734" alt="image" src="https://github.com/user-attachments/assets/b37cb0e4-d388-4b6f-8982-4dc757fd2f27" />

Having multiple websites running on a IIS server can be problematic to make migraiton to a new machine, besides copying the data you have to recreate new application pool's and website.

To simplify the process on machines in the same domain we have two simple scripts:

--- The origin script automatically exports all IIS Application Pools, Websites, and Anonymous Authentication configurations, copies them to the target server, and remotely triggers the import process.
https://github.com/covtandre/IIS_Migration/blob/main/Origin_Script


--- The destination script clears any existing IIS configuration, imports the exported XML files, reapplies Anonymous Authentication settings, and restarts IIS to finalize the migration.
https://github.com/covtandre/IIS_Migration/blob/main/Destination_Script

Full article:
https://blog.cyber-lit.net/2025/10/05/export-and-import-all-iis-application-pools-and-websites-between-servers/


