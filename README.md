To use the script:

1. Set your configuration:
```python
SYMBOL = "your_symbol"
ACCOUNT = "your_account_number"
PASSWORD = "your_password"
SERVER = "your_broker_server"
```

2. Run before market open (it will wait for 9:30 AM ET)

The strategy will:
1. Wait for market open
2. Analyze first 5 minutes
3. Place trade if momentum is strong enough
4. Set stop loss and take profit
5. Monitor position
6. Close after 1 hour if not already closed by SL/TP

Important notes:
- Test in demo account first
- Momentum threshold of 0.3 can be adjusted
- Stop loss and take profit multipliers can be modified
- The strategy automatically exits after 1 hour
- Proper risk management with 1% risk per trade
