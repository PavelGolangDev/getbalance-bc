��������� �������� �� ����� Go, � ����� ���������� Visual Studio Code. 
��� ���� ��� �� �� ���������, ��������� ������������� Go.
��������� ����������� ������� ��������� ������ � ������� ��������������. ���� Go ������ � ��������� ���������� PATH,�� ��������� �������� ��������� "go build GOLANG.go".
���� � ���������� PATH ������ �� ���������, ����� C:\(������������ go)\go.exe run C:\(������������ �����)\GOLANG.go

� ��������� ���������� �������� � �������������� ���� ������ BoltDB. ������ ������ ����� ��������� � �����, � ����� ��������
��������� �������� �����������. �������� ��������� �� ������ ���������: 1) ����������� ���� ���� ������ 2) �������� ������� � ��� ���������
3) ���� �������� ��� ������������: - ��������� ����� ��������� - tip ��������������� �� ��� ���������� ������������ � �� �����.
4) ���� ��������� � ����� ���: - ��������� ������� ���� � ����������� � ���� ������ - ��� ����������� ����� ����������� ��� ��� ���������� �����.
� ��������� ��� �� ���������� ��������� �������� ������.
� ������� ����������� ���������� � ������� �� �������. ������� �� ������� ��������������� ����������.
�� ������� ����� �������� ������� 10 BTC. ����������� ������� createblockchain -address "��������". ������� ������� ���� 
� ������� �The Times 03/Jan/2009 Chancellor on brink of second bailout for banks�. 
������� getbalance -address "��������" ������� ������ �� ������.
������� send -from "��������" -to "��������" -amount "���-�� BTC". ������� ����, � ����������� ��������.
������� printchain ������� ��� ����� � ���������� ��� ���.
����� ���� �������� �� ������������ ��������.


Programm developed by Go language, in the development environment Visual Studio Code.

In programm realize blockchain using a database BoltDB. Data store in file and aft�r closing progress saved.
Blockchain created by algorithm: 1) Open database file 2) Check for blockhain 3) If blockchain present - create
new instance and flag "tip" set in hash last save in database block. 4) If there is no blockchain in the file -
create genesis block and save in database - genesis block hash save as hash last saved block in database.
In the program is implemented CLI interface.
The project also implemented transactions and awards for mining. The reward is set by a constant.
For mining genesis block - reward 10 BTC.
Implemented command (createblockhain -address "Name"). Create a genesis block.
Command (getbalance -address "Name"). Shows the balanc�.
Command (send -from "Name" -to "Name" -amount "amount BTC") - creat transfer transaction block.
Command (printchain) displays all blocks.
Part of the code is cut for commercial reasons.


	Legal (Copyright) 2018-2019 @PavelGolangDev
	All Rights Reserved
