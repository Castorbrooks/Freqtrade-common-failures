# Freqtrade – Common Failures & Fixes

This repository documents the most frequent problems
that cause Freqtrade bots to stop trading or behave incorrectly.

Focus: **diagnosis and repair**, not strategy creation.

---

## Most common Freqtrade failures

• Exchange API 429 (rate limit exceeded)
• Invalid nonce / timestamp errors
• Orders created but never filled
• Bot runs but no trades executed
• Dry-run works, live trading fails
• Pair whitelist issues
• WebSocket disconnects

---

## Why these failures happen

• Exchange-side rule changes
• Poor API error handling
• Incorrect config values
• Strategy logic edge-cases
• Missing reconnect logic
• Latency or timing mismatch

---

## How fixes are done (Safe Process)

• No API keys required  
• No exchange login needed  
• Log-based diagnosis only  
• Sandbox / dry-run verification  
• Minimal logic patch (not full rebuild)

---

## Example Failure Case

**Issue:**  
Freqtrade bot running but no trades placed

**Root cause:**  
Pair whitelist filtered out all tradable pairs

**Fix:**  
• Config correction  
• Validation added  
• Safe restart logic

**Result:**  
Bot resumed trading normally

---

## Typical repair time

⏱ 30 – 90 minutes  
💰 Paid repair, same-day completion

---

## Who should use this

• Traders stuck with Freqtrade errors  
• Bot owners facing sudden failures  
• Developers inheriting broken bots  
• Teams needing urgent stabilization

---

If your Freqtrade bot stopped working,
it can usually be fixed quickly.
