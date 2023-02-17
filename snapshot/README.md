# COREUM DAILY SNAPSHOT
coreum network

```console
sudo systemctl stop cored
planqd tendermint unsafe-reset-all --home $HOME/.core/coreum-testnet-1 --keep-addr-book
curl -L https://snapshot.crxaa.my.id/snapshot/coreum/cored-snapshot.tar.lz4 | lz4 -dc - | tar -xf - -C $HOME/.core/coreum-testnet-1 --strip-components 2
sudo systemctl start cored && journalctl -u cored -f --no-hostname -o cat
```