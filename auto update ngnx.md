# planq
planq network
Auto update nginx explrer

  ```console
  rm -rf $HOME/explorer/dist
  rm -rf /usr/share/nginx/html/*
  cd ~/explorer
  yarn && yarn build
  npm run build-only
  cp -r $HOME/explorer/dist/* /usr/share/nginx/html
  cp -r $HOME/css /usr/share/nginx/html
  nginx -s reload
  ```
