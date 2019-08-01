Программа написана на языке Go, в среде разработки Visual Studio Code. 
Для того что бы ее запустить, требуется установленный Go.
Программа запускается помощью командной строки с правами администратора. Если Go введен в системную переменную PATH,то требуется написать следующее "go build GOLANG.go".
Если в переменную PATH ничего не добавляли, тогда C:\(Расположение go)\go.exe run C:\(Расположение файла)\GOLANG.go

В программе реализован блокчейн с использованием базы данных BoltDB. Теперь данные будут храниться в файле, и после закрытия
программы прогресс сохраняется. Блокчейн создается по такому алгоритму: 1) Открывается файл базы данных 2) Проверка наличия в нем блокчейна
3) Если блокчейн там присутствует: - создается новый экземпляр - tip устанавливается на хэш последнего сохраненного в БД блока.
4) Если блокчейна в файле нет: - создается генезис блок и сохраняется в базу данных - хэш генезисного блока сохраняется как хеш последнего блока.
В программе так же реализован интерфейс командой строки.
В проекте реализованы транзакции и награды за майнинг. Награда за майнинг устанавливается константой.
За майнинг блока генезиса награда 10 BTC. Реализована команда createblockchain -address "Название". Создает генезис блок 
с текстом “The Times 03/Jan/2009 Chancellor on brink of second bailout for banks”. 
Команда getbalance -address "Название" выводит баланс по адресу.
Команда send -from "Название" -to "Название" -amount "Кол-во BTC". Создает блок, с транзакцией перевода.
Команда printchain выводит все блоки и информацию про них.
Часть кода вырезана по коммерческим причинам.


Programm developed by Go language, in the development environment Visual Studio Code.

In programm realize blockchain using a database BoltDB. Data store in file and aftеr closing progress saved.
Blockchain created by algorithm: 1) Open database file 2) Check for blockhain 3) If blockchain present - create
new instance and flag "tip" set in hash last save in database block. 4) If there is no blockchain in the file -
create genesis block and save in database - genesis block hash save as hash last saved block in database.
In the program is implemented CLI interface.
The project also implemented transactions and awards for mining. The reward is set by a constant.
For mining genesis block - reward 10 BTC.
Implemented command (createblockhain -address "Name"). Create a genesis block.
Command (getbalance -address "Name"). Shows the balancе.
Command (send -from "Name" -to "Name" -amount "amount BTC") - creat transfer transaction block.
Command (printchain) displays all blocks.
Part of the code is cut for commercial reasons.


	Legal (Copyright) 2018-2019 @PavelGolangDev
	All Rights Reserved
