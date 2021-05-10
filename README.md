# webturtle
A web miner for FTSCoin (based on TurtleCoin Webminer)

#### Working demo: [https://trtlminer.herokuapp.com](https://trtlminer.herokuapp.com)

## How to include to your website
In order to implement the miner to your website you have to do the following, easy steps:

 - Download our script and add it to your website  
  `<script src='turtleminer.js'></script>`  

 - Edit the configuration
  ```
const config = {
	pool: "www.ftscoinpool.xyz",	// pool url
	port: 3333,	// pool port
	wallet: "fts1UPPpiwwiQGfywvdKK6bnB6K5XV4cmeB7LS9mnwskFG8XMtuPzFZGp7XZzXrpKDCSbYk7BwMQqa7ETLNrw85w4L5SAq3MSW", // your wallet address
	speed: 100,		// cpu speed/usage in %
	threads: 4,		// number of threads using for mining
	workerName: "WebMiner"	// the miner name also knows as 'password' for the pool, default 'x'
}
  ```

  - Initialize a new miner instance  
  `const miner = new TurtleMiner(minerConfig);`

  - Start mining whenever you want:  
  `miner.start();`

  - Stop mining whenever you want:  
  `miner.stop();`
