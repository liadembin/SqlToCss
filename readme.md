# a new side project, inspired by the primeagens video - https://youtu.be/R9tLkhkDtWc
# Currently this is implemented in python, will be translated to go as an attempt to learn go 
# attempting to support: SELECT,UPDATE,LIMIT,JOINS(taking propertys from diffrent selector, will probably be by a shared class) AS WELL AS A VARIABLE Table, 
# mysql syntax for the most part
# delete,creating table from table not yet supported.
# example SQL and its desired output
use class;
# creating table from another will not be supported
# default values for all will just be to not exist ex: 
# if width will not be passed, the resulting css will not have it 
# so skiping the table create may be possible - not decided
create table myDiv (
 	display varchar(255),
	width varchar(255), # not int because of units
	height varchar(255), #same
	position varchar(255)
)
#each table has a inferd id int field to support limit and where
insert into myDiv(
	(display,position,width,height)	values (flex,absoulte,128px,256%)	
)
update myDiv set position = "relative" where id = 1

# not using where as the table will be 1 row 
# consider moving everything to be part of one Table rather than many tables in many databases
# because object shape may be inferd 
# for now Im implemeing databases meaning diffrent selection methods, each table is selector 
# as it is the naive first idea.
