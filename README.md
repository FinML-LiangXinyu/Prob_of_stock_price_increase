# 股价上涨概率

## 对数正态分布假设与股价上涨概率

$t$ 时刻的股价服从对数正态分布 $\Delta lnSt\sim N(\mu\Delta t,\sigma^2\Delta t)$

故有股价上涨概率：

$P\left(S_T\geq S_t\right)=P\left(lnS_T\geq lnS_t\right)=P\left(\Delta lnSt≥0\right)=P\left(\frac{\Delta lnS_t-\mu\Delta t}{\sigma\sqrt{\Delta t}}\geq-\frac{\mu}{\sigma}\sqrt{\Delta t}\right)=N\left(\frac{\mu}{\sigma}\sqrt{\Delta t}\right)$

## 几何布朗运动与股价上涨概率

$t$ 时刻的股价遵循几何布朗运动 $S_t=S_0e^{\left(\mu-\frac{1}{2}\sigma^2\right)t+\sigma W\left(t\right)}$

$T$ 时刻的股价遵循几何布朗运动 $S_T=S_0e^{\left(\mu-\frac{1}{2}\sigma^2\right)T+\sigma W\left(T\right)}$

则 $T$ 时刻的股价 $S_T$ 可以用 $t$ 时刻的股价 $S_t$ 表示为： 

$S_T=S_te^{\left(\mu-\frac{1}{2}\sigma^2\right)\mathrm{\Delta t}+\sigma\Delta W\left(t\right)}$

故有股价上涨概率：

$$P\left(S_T\geq S_t\right)=P\left(lnS_T\geq l n S_t\right)=P\left(\mathrm{\Delta ln}S_t\geq0\right)=P\left(\left(\mu-\frac{1}{2}\sigma^2\right)\mathrm{\Delta t}+\sigma\Delta W\left(t\right)\geq0\right)=P\left(\mathrm{\Delta W}\left(t\right)\geq-\frac{\left(\mu-\frac{1}{2}\sigma^2\right)\mathrm{\Delta t}}{\sigma}\right)=P\left(\frac{\mathrm{\Delta W}\left(t\right)}{\sqrt{\mathrm{\Delta t}}}\geq-\frac{\left(\mu-\frac{1}{2}\sigma^2\right)\mathrm{\Delta t}}{\sigma\sqrt{\mathrm{\Delta t}}}\right)=N\left(\frac{\left(\mu-\frac{1}{2}\sigma^2\right)}{\sigma}\sqrt{\mathrm{\Delta t}}\right)$$
