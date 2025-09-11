
## Ex 1

![[Pasted image 20250910105905.png]]
Both can fail, failing silently all messages that should have been sent are omitted, whereas 

---

## Ex 2

![[Pasted image 20250910105917.png]]
```
Implements:
	StubbornLink, instance sl

Uses:
	FairLossP2PLink, instance p2p

upon event <sl, Init> do
	stop := false
	
	while not stop then
		trigger <p2p, Send | sl>

upon event <p2p, Deliver>
	stop := true

```

---

## Exercise 3

![[Pasted image 20250910110009.png]]

Have a perfect P2P link and send a heartbeat request to each process. If a process does not answer within the max time frame then we can be sure it is dead because there is a fixed delay for synchronous system. 

---

## Exercise 4

![[Pasted image 20250910110739.png]]

You know that a request will be answered within one week, and as such there is timed failure detection. 

---

## Exercise 5

![[Pasted image 20250910111355.png]]

Even with a synchronous system with perfect P2P we cannot determine whether the heartbeat from a process is correct since it may crash arbitrarily, and give whatever answer to the failure detector. 

---

## Exercise 6

![[Pasted image 20250910112509.png]]

| uptime | total downtime per month |
| ------ | ------------------------ |
| 90%    | 74.4H                    |
| 99%    | 7.4H                     |
| 99.9%  | 0.74H                    |
| ...    | ...                      |

---

## Exercise 7

![[Pasted image 20250910112634.png]]
![[Pasted image 20250910112646.png]]

| uptime | downtime per year |
| ------ | ----------------- |
|        |                   |

---

## Exercise 8

![[Pasted image 20250910114807.png]]

All messages pass through link 6 since it is a bottleneck.

---

## Exercise 8.1

![[Pasted image 20250910115040.png]]
You would need all links connecting from 1 to 2 to have three edges. You can imagine a fully connected neural network with three neurons per layer. If a layer has less than 2 neurons you can remove them and the connection fails.
