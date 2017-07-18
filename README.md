# Repository for quick experimental tools

- [``mycookies <hostname>``](mycookies)

  Load cookies from Chrome storage for a given hostname. Can be used with curl or wget to load things from internet using credentials of
  my Chrome browser:
  
  ```
  $ curl -H `mycookies github.com` http://github.com/Username/MyPrivateRepo/blob/...
  ```

- [``csssel <query>``](csssel)

  Filter html based on css selector

  For example:

  ```
  $ curl https://www.bbc.co.uk | csssel -t '.top-story__title
  Guilt 'eats up' brothers of murder victim Sarah Payne
  England take on South Africa in World Cup semi-final
  ...
  ```

- [``github-browse <filename>``](github-browse)

  Open a file in a git repository tree on github.

  ```
  $ github-browse README.md
  <opens Chrome window pointing to https://github.com/skyjur/utils/blob/master/README.md>
