# Deployments

## Rewards

The two main mining mechanism are `Swap Mining` and `LP Mining`

### Swap Mining

`Swap Mining` allows users that use swap to balance the bretton pool to receive `BRET` rewards proportionally to their swap volume. Whether a swap is helping to balance of pool (i.e elligable for reward) is determined by the stateless and upgradable `SwapMiningRewardsCalc`.

### LP Mining

LP mining allows users stake their LP tokens (e.g `BRET/USDT`, `bretUSD`) to earn more `BRET`.

### Vault

`BRET` holder can enter `Vault` to earn governance right to the Bretton protocol. All mined `BRET` rewards enter the vault first by default upon claim. Users can choice to exit anytime they wish.

Upon exiting vault, a 10% exit fee is taken and distributed as following:
- 2% of withdraw amount is burnt.
- 4% is sent to DAO and becomes apart of `protocol controlled value (PCV)`.
- 4% is distributed to the rest of the vault pool.

## DAO

The DAO `Treasury` receives token from `swapping fees` and `Vault`, and performs buyback and add to LP.

For example, the treasury receives `USDT` from the bretton pool as swapping fee. It then sells half of the `USDT` for `BRET`, and add to `USDT/BRET LP`.

---

![Alt text](diagram.png)

## Contract Addresses

Addresses are categorized by network ID.

[address.js](address.js)
