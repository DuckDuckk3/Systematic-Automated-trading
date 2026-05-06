Neutralization: None | Universe: TOP3000. These alphas works well on smaller universes with cleaner data. Sub-universe shape might be low. 
- `rank(cashflow / assets)`
- `rank(cashflow/enterprise_value)`
- `rank((cashflow - interest_expense - capex) / assets)`
- `rank(mdl77_liquidityriskfactor_growdura / enterprise_value)`
- `rank(ebitda - capex / enterprise_value)`

Neutralization: Subindustry | Universe: TOP3000.
- `group_neutralize(rank(liabilities / assets) + rank(cogs / assets), subindustry)` performs well
- `rank(inventory / capex)`

