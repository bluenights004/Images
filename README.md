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
### 4. Triangle facing right

<details>
<summary> Click to reveal</summary>

This is the hidden content that becomes visible when the triangle is clicked.

- You can add a list
- Or any other Markdown content
- Including **bold** text and [links](https://example.com).

</details>

