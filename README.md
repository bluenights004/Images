# Audit Report 
Various tricks in markdown used for writing audit finding report

### 1. Web Link

[sample](https://audits.sherlock.xyz/contests)

### 2. Pasting from source document

>Chain re-org and network liveness issues are not valid.

### 3.  Difference in code

```Diff
vault.updateGlobalPositionData({
-           price: position.lastPrice,
+           price: currentPrice,
            marginDelta: -(int256(position.marginDeposited) + positionSummary.accruedFunding),
            additionalSizeDelta: -int256(position.additionalSize)
        });
```
