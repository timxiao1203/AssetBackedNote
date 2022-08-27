# Asset Backed Note

A asset backed securitization note allows the holder to purchase co-ownership interests in a revolving pool of credit card receivables. To fund the acquisition of the interests in the revolving pool, the trust issued Asset-Backed Notes, in a number of different series. A share of future collections of credit charge receivables, to which the trust is entitled, is used to pay the interest and the principal of the notes. Accrued interest can be computed like https://finpricing.com/lib/FiBondAccrual.html)

At this time the deal has entered its liquidation period, during which all allocable collections remaining after the payment of interest are used to repay the principal. For this reason, only the portion of the model relevant to the liquidation period

The valuation is updated from time to time to account for changes in certain parameters, most notably the liquidation (prepayment) rate and the pool balance.

Some spot checks were performed on certain formulae (notably the discount factors) and sensitivity to certain parameters was examined by observing the results of the computations as the input parameters varied.

The valuation makes the assumption that the future values of these parameters will be unchanged until the final payment date. Subsequently, the calculator performs a deterministic computation consisting of calculating the future cashflows in the waterfall and discounting them.

We first focus on the principal payment, which is the pro-rated entire senior principal payment Z. This last amount is the allocated collection amount U, less the aggregate (senior and subordinate) interest V. 

Both the aggregate interest and the allocated collection amount depend on the remaining aggregate (senior and subordinated) principal X. Each month during the liquidation period the aggregate principal is reduced by the senior principal payment Z, unless it falls below a certain amount, which will trigger the cleanup prepurchase option, so that the entire remaining principal is paid off immediately (not shown in the formulae for simplicity). 

The aggregate interest applies the weighted coupon rate to the aggregate principal, while the interest payment AF applies the senior coupon rate to the (pro-rata) remaining senior principal. The formulas guarantee that the principal payment never exceeds  the remaining principal. 

The remaining pro-rata senior principal AF and the remaining senior principal AA are reduced each month by the corresponding principal payments. The formula defines the collections allocated. The collections consist of the principal portion and the interest portion. 

References:

https://osf.io/eg6mv/download

