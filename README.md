## Notes / To do

* Scaling the data?
* Donnees fondamentales?
* Leverage, lower bound on bank account
* tests unitaires
* typical buy_rate and sell_rate = 0.1%

## Requirements

* Python>=3.6
* numpy
* pandas
* jupyter
* sklearn
* matplotlib
* seaborn
* pytorch
* yfinance
* gym

```shell
pip install .
```
 ## Example 
 ### __Create a model__, train it, and save the trained model. If you have GPUs, they will automatically be used.

```shell
python main.py \
--initial_cash 10000 \
--buy_rate 0.01 \
--sell_rate 0.01 \
--sac_temperature 2.0 \
--limit_n_stocks 50 \
--lr_Q 0.003 \
--lr_pi 0.003 \
--tau 0.005 \
--batch_size 256 \
--layer1_size 256 \
--layer1_size 256 \
--n_episodes 10 \
--seed 42 \
--memory_size 1000000 \
--initial_date 2010-01-01 \
--final_date 2020-12-31 \
--auto_temperature \
--gpu_devices 0 1 2 3 \
```
## License
[Apache License 2.0](https://github.com/MatthieuSarkis/stock/blob/master/LICENSE)