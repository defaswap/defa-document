# 🚜 Yield Farming

![](<../../.gitbook/assets/image (20).png>)

Yield Farms allow users to earn Defa while supporting Defa platform by staking LP Tokens.

Check out our [How to Use Farms guide](how-to-use-farms.md) to get started with farming.

Learn [how to find Farm smart contracts](./)

Check out this great [article about Impermanent Loss ](https://academy.binance.com/en/articles/impermanent-loss-explained)from Binance Academy to learn more.

## **Reward calculations**

Yield Farm APR calculations include both:

* **LP rewards APR** earned through providing liquidity and;
* **Farm base rewards APR** earned staking LP Tokens in the Farm.

Why? Because when you stake your LP tokens in a farm to earn Defa, you're still providing liquidity to the liquidity pool, so you earn LP rewards as well!

![](<../../.gitbook/assets/image (21).png>)

So how do we calculate those figures?

### Calculating Farm Base Reward APR

The **Farm Base APR** is calculated according to the farm multiplier and the total amount of liquidity in the farm -- this is the amount of Defa distributed to the farm.

### Calculating LP Reward APR

On top of that, farmers receive **LP rewards** for providing liquidity. Here's an example of calculating **LP rewards**:

![](<../../.gitbook/assets/image (2).png>)

In the WBNB/BUSD pair above, we see these values:

**Liquidity:** $387.42M **Volume 24H:** $96.97M **Volume 7D:** 709.73M

* Calculate yearly fees
* Use the 24H volume to calculate the **fee share** of liquidity providers in the pool (based on the 0.17% trading fee structure): $96,970,000\*0.17/100 = **$164,849**
* Next, use that **fee share** to estimate the projected **yearly fees** earned by the pool (based on the current 24h volume): $164,849\*365 = **$60,169,885**
* We can now use the yearly fees to calculate the **LP rewards APR:** That's **yearly fees** divided by **liquidity:** ($60,169,885/$387,420,000)\*100 = **15.53% LP reward APR**
