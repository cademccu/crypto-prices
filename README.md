# crypto-prices
Get the prices of your favorite cryptos with a simple command line script

### Usage
Get your API key from https://coinmarketcap.com/api/

Include this in a file called KEY.py of the format:
```
# KEY.py
API_KEY="your_key_here"
```

Optionally, you can include a dictionary named CONVERT with a string:float value with the number of
a type of coin you hold. This will be included after the regular output.

```
CONVERT = {
	"ETH":1.43
}
# this will display your ETH holdings as 1.43 coins.
```

Sample output from this:

```
ETH : 3205.43$
	[OWNED] ETH : 803.80$
BTC : 44394.59$
```


This will be imported into the file, so it is important that this file is in the same directory as the 
script, or you include the path to the import. You can also write this directly into the script,
an option that would be easier if you never put it on github.

If using as script:
```
chmod +x crypto
```

This default just calls and sorts for Ethereum and Bitcoin.

Edit the comma-seperated string at the top of symbols to get more or less.
```
SYMBOLS = "ETH,BTC"
```

