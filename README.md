# basell
Measuring Block Time Stability on Base (Python)  I pulled block timestamps to see how stable the chain is under load.
blocks = [w3.eth.get_block(i) for i in range(8000000, 8000010)]
times = [b.timestamp for b in blocks]
print(times)
Base remains extremely consistent — great for predictable UX.
