
# faStock-Chain Snapshot

Quick instructions on how to install the faStock-Chain snapshots.

## mainnet
Download URL: 
  - [fastock-chain-v0.16.3-mainnet-20210127-height_275913.tar.gz](https://ok-public-hk.oss-cn-hongkong.aliyuncs.com/cdn/fastock-chain/snapshot/fastock-chain-v0.16.3-mainnet-20210127-height_275913.tar.gz)

## Unpack the snapshot file for cosmos
```shell
mv ~/.fastock-chain-daemon/data ~/.fastock-chain-daemon/data-bak
# rm -rf ~/.fastock-chain-daemon/data
cd ~/.fastock-chain-daemon 
tar -zxvf fastock-chain-$version-$date-$height_xxx.tar.gz
```
