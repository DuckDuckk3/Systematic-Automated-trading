Neutralization: Industry | Universe: TOP3000
- `-rank(ts_arg_min(returns,5))`
- `group_neutralize(rank(ts_decay_linear(-(ts_zscore(volume,20)*returns),5)),sector)`
