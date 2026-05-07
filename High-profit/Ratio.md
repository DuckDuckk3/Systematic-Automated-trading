Neutralization: None | Universe: TOP3000. These alphas works well on smaller universes with cleaner data. Sub-universe shape might be low. 
- `rank(cashflow / assets)`
- `rank(cashflow/enterprise_value)`
- `rank((cashflow - interest_expense - capex) / assets)`
- `rank(mdl77_liquidityriskfactor_growdura / enterprise_value)`
- `rank(ebitda - capex / enterprise_value)`

Neutralization: Subindustry | Universe: TOP3000.
- `group_neutralize(rank(liabilities / assets) + rank(cogs / assets), subindustry)` performs well
- `rank(inventory / capex)`
- `-ts_decay_linear(group_neutralize(rank(ts_delta(cashflow, 252) / enterprise_value), industry), 30)`
- `-ts_decay_linear(group_neutralize(rank(cashflow / enterprise_value), subindustry), 10)`
- `-rank(cashflow / sales)`
- `rank(cogs/assets)`

