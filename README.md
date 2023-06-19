# uniV3 tron 部署：

## usage

### compile

```sh
$ truffle compile
```

### deploy

```sh
$ tronbox migrate --f 2 --to 2 --network nile
```

PS: 
1. 合约本身存在的问题，见TODO.md
2. tronbox限制合约名长度为32个字符，故将 NonfungibleTokenPositionDescriptor 改为 NftPositionDescriptor.
3. NonfungibleTokenPositionDescriptor 部署需要优先部署lib合约 NftDescriptor，然后通过link的方式 部署 NonfungibleTokenPositionDescriptor
4. 其他合约名暂未改动
