Programm developed by Go language, in the development environment Visual Studio Code.

In programm realize blockchain using a database BoltDB. Data store in file and aftår closing progress saved.
Blockchain created by algorithm: 1) Open database file 2) Check for blockhain 3) If blockchain present - create
new instance and flag "tip" set in hash last save in database block. 4) If there is no blockchain in the file -
create genesis block and save in database - genesis block hash save as hash last saved block in database.
In the program is implemented CLI interface.
The project also implemented transactions and awards for mining. The reward is set by a constant.
For mining genesis block - reward 10 BTC.
Implemented command (createblockhain -address "Name"). Create a genesis block.
Command (getbalance -address "Name"). Shows the balancå.
Command (send -from "Name" -to "Name" -amount "amount BTC") - creat transfer transaction block.
Command (printchain) displays all blocks.
Part of the code is cut for commercial reasons.


	Legal (Copyright) 2018-2019 @PavelGolangDev
	All Rights Reserved
