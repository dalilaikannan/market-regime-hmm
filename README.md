# market-regime-hmm

A 3-state Gaussian Hidden Markov Model trained on daily SPY log returns and VIX data from 2000 to present. The model learns to segment market history into regimes — bull, bear, etc. — without any labeled training data. Parameters are fit via Baum-Welch (EM) and state sequences decoded with Viterbi.

The regime chart correctly surfaces the dot-com crash, 2008 financial crisis, COVID shock, and 2022 drawdown as distinct states. Built with `hmmlearn`, `yfinance`, `pandas`, and `matplotlib`.
