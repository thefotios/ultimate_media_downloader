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
