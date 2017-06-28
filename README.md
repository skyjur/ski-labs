# Repository for quick experimental tools

- [``mycookies <hostname>``](mycookies)

  Gets cookies from Chrome storage for a given hostname. For example use with curl to retrieve a file from private repository:
  
  ```
  $ curl -H `mycookies github.com` http://github.com/Username/MyPrivateRepo/blob/...
  ```

- [``csssel <query>``](csssel)

  Filter html based on css selector

  For example:

  ```
  $ curl https://www.bbc.co.uk | csssel -t '.top-story__title
  ```
