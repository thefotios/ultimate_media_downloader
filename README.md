1. Create system users

  ```
   useradd -r -U couchpotato
  ```

1. Set ACLs
  1. CouchPotato

    ```
    setfacl --set-file acls/CouchPotatoServer.acl CouchPotatoServer
data/CouchPotatoServer
    ```

1. Modify Init Scripts
  1. CouchPotato
    * Point CouchPotato to use your new data directory by adding the
following line to whichever init script you use:

      ```
      --data_dir=/home/your_user/ultimate_media_downloader/data/CouchPotatoServer
      ```

1. Add the Init scripts for your OS
