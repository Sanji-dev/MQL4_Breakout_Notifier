# MQL4 Breakout Notifier

Breakout indicator build on MQL4 langage sends push notifications to the mobile terminals according to multiple condition based on Donchian indicator, RSI, ATR and moving average.

## Requirement

- Install [MetaTrader 4](https://www.metatrader4.com/fr) for computer
- Install [Metatrader app](https://www.metatrader4.com/fr/mobile-trading/android) on mobile
- Demo or real account from any Broker

## Install Indicator

1. Navigate to “File” in the upper left hand corner and then select "Open Data Folder"
2. From there navigate to the folder called "MQL4"
3. From there navigate to the folder called "Indicators"
4. Drag and drop the indicators that you want to install into this folder
5. Close and open MT4 plateform

## Push notification

### How to use
**Find your MetaQuote ID**
1. Open the "MT4" App.  When the App opens the first time, select "OK" to allow Notifications.
2. Select "Settings" at bottom of page.
3. Select "Messages".
4. Find your MetaQuotes ID# at the bottom of the page.

**Set your MetaQuote ID in your MetaTrader 4 plateform**
1. Open Your MetaTrader 4 Platform and Select Tools->Options
2. In "Notifications" Tab, Enter Your MetaQuotes ID # and Select OK
3. Refresh file

### Function code
```python
SendNotification((string)Symbol()+" Cassure Haussière !");
```

### Note
Strict use restrictions are set for the SendNotification() function: no more than 2 calls per second and not more than 10 calls per minute. Monitoring the frequency of use is dynamic. The function can be disabled in case of the restriction violation.

SendNotification() function **does not work in the Strategy Tester**.






