SimpleSVNServer
=================
 
Simple Alpine based svn server.

This is a bare bones svn server which exposes a local svn volume mounted to `/svn`.

The server includes an svnservice which is run in the forground and can be monitored with `docker logs -f <container_name>`

## To run a simple server

  ```
  docker run -d -p 3690:3690 neiltheblue/simplesvnserver \
  -d -v <local_path>/svn:/svn 
  -p 3690:3690
  ```
  
