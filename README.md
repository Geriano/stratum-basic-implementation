### Stratum basic implementaion 
This is basic of stratum protocol where is used by bitcoin for comunicate between miner and pool.
Contains two of binnary:
- first is `server` is for accepting connection for one or more miner then distribute to other mining pool.
- second is `client` which is basic implementation of miner protocol comunication between our server. this is very usefull for simulating miner rig/tool eg asic miner

## Step to run
- clone this repo then go to folder
```bash
git clone https://github.com/Geriano/stratum-basic-implementation
cd stratum-basic-implementation
```
- run the server go to `server` directory and then run the server
```bash
cd server 
cargo run --release
```
- now the server can accept miner connection on port 5098
- run the client/miner 
```bash
cd ../client # we are in server directory
cargo run --release
```
- now the miner can working for job given by server
- you can simulate more then once miner, just run it the client again

## Todo
- Connecting the server into pool (eg. nicehash)
