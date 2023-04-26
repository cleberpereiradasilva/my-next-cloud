# my-next-cloud

My Private Cloud using Oracle Cloud and Nextcloud

## Instaling Nextcloud

1. Clone this repository
2. Edit file `docker-compose.yml`

   - Set in **nextcloud** service:
     - NEXTCLOUD_ADMIN_USER=**YOUR_USERNAME**
     - NEXTCLOUD_ADMIN_PASSWORD=**YOUR_PASSWORD**
     - NEXTCLOUD_TRUSTED_DOMAINS=**YOUR_IP_ADRRESS**
   - Set in **postgres_sql** service:
     - POSTGRES_USER=**DATABASE_USER_NAME**
     - POSTGRES_PASSWORD=**DATABASE_PASSWORD**

3. Edit file `create_database.sql`

   `CREATE DATABASE db_my_nextcloud OWNER **<DATABASE_USER_NAME>**;`
