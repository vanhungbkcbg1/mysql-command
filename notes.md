backup database
command tong quat
mysql -h [host] -u [user_name] -p [options] [database] [table] > [filename].sql

back up ca du lieu va schema

mysql -h [host] -u [user_name] -p [database] [table] > [filename].sql
example
mysql -h 127.0.0.1 -u test -p test > test_bk.sql

backup schema only
mysql -h [host] -u [user_name] -p --no-data [database] [table] > [filename].sql
example
mysql -h 127.0.0.1 -u test -p --no-data test > nodata.sql

backup data only

mysql -h [host] -u [user_name] -p --no-create-info [database] [table] > [filename].sql

example
mysql -h 127.0.0.1 -u test -p --no-create-info test > test.sql

backup with individual table
mysql -h 127.0.0.1 -u test -p --no-create-info test posts users > test.sql 

cau lenh tren la backup data cua 2 table posts va users

back up except table nao do
examle

mysql -h 127.0.0.1 -u test -p --no-create-info  test --ignore-table test.posts >test.sql

trong menh de tren thi menh de ignore-table phai chi dinh ca datatable.table muon ignore 



dump options
https://dev.mysql.com/doc/refman/8.0/en/mysqldump.html#mysqldump-option-summary
