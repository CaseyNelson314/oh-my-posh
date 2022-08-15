# oh-my-posh original theme

## 🤔description

oh-my-posh 自作テーマ json

![image](https://user-images.githubusercontent.com/91818705/184508428-6f5720dc-7a3c-45b7-b39c-ad6c556f596b.png)


## 📝memo

### oh-my-posh install

  - `winget`コマンドでインストール

      ```sh
      winget install oh-my-posh
      ```
    
  - シェル起動時のプロファイル設定

      ```sh
      notepad $PROFILE
      ```
       
    プロファイルがない場合
    
      ```sh
      New-Item -ItemType File -Path $PROFILE -Force
      notepad $PROFILE        
      ```

      以下を記述

      ```sh
      oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\paradox.omp.json" | Invoke-Expression
      ```
      
      プロファイルが読み込まれない場合

      ```sh
      Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
      ```
        
  - フォントのインストール
    
      oh-my-posh は 以下の専用のフォントを使って表示しています
        
      https://www.nerdfonts.com
      
  - フォント設定
  
      設定 > 既定値 > 外観 > フォントフェイス

### customize

- テーマの変更

    `$PROFILE` 内の `paradox.omp.json`のファイル名を変更する

-  テーマ一覧

    https://ohmyposh.dev/docs/themes

- 追加

   追加するjsonファイルは `$env:POSH_THEMES_PATH` ディレクトリ内に配置する
   ```sh
   start $env:POSH_THEMES_PATH
   ```

- 基本的に oh-my-posh [公式ドキュメント](https://ohmyposh.dev/docs) の`🌟Segments`を見ることでカスタマイズが可能

- セグメントリスト内を変更することで外見が変更される
