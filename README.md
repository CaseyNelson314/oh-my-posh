# oh-my-posh original theme

## ð¤description

oh-my-posh èªä½ãã¼ã json

![image](https://user-images.githubusercontent.com/91818705/184508428-6f5720dc-7a3c-45b7-b39c-ad6c556f596b.png)


## ðmemo

### oh-my-posh install

  - oh-my-posh ã¤ã³ã¹ãã¼ã«

      ```sh
      winget install oh-my-posh
      ```
    
  - ã·ã§ã«èµ·åæã®ãã­ãã¡ã¤ã«è¨­å®

      ```sh
      notepad $PROFILE
      ```
       
    ãã­ãã¡ã¤ã«ããªãå ´å
    
      ```sh
      New-Item -ItemType File -Path $PROFILE -Force
      notepad $PROFILE        
      ```

      ä»¥ä¸ãè¨è¿°

      ```sh
      oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\paradox.omp.json" | Invoke-Expression
      ```
      
      ãã­ãã¡ã¤ã«ãèª­ã¿è¾¼ã¾ããªãå ´å

      ```sh
      Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
      ```
        
  - ãã©ã³ãã¤ã³ã¹ãã¼ã«
    
      oh-my-posh ã¯ ä»¥ä¸ã®å°ç¨ã®ãã©ã³ããä½¿ã£ã¦è¡¨ç¤ºãã¦ãã¾ã
        
      https://www.nerdfonts.com
      
  - ãã©ã³ãè¨­å®
  
      è¨­å® > æ¢å®å¤ > å¤è¦³ > ãã©ã³ããã§ã¤ã¹

### customize

- ãã¼ãã®å¤æ´

    `$PROFILE` åã® `paradox.omp.json`ã®ãã¡ã¤ã«åãå¤æ´ãã

- ãã¼ãä¸è¦§

    https://ohmyposh.dev/docs/themes

- è¿½å 

   è¿½å ããjsonãã¡ã¤ã«ã¯ `$env:POSH_THEMES_PATH` ãã£ã¬ã¯ããªåã«éç½®ãã
   ```sh
   start $env:POSH_THEMES_PATH
   ```

- åºæ¬çã« oh-my-posh [å¬å¼ãã­ã¥ã¡ã³ã](https://ohmyposh.dev/docs) ã®`ðSegments`ãè¦ããã¨ã§ã«ã¹ã¿ãã¤ãºãå¯è½

- ã»ã°ã¡ã³ããªã¹ãåãå¤æ´ãããã¨ã§å¤è¦ãå¤æ´ããã
