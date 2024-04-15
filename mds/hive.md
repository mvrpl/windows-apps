#### GENERAL
|||
|-|-|
`LOAD DATA LOCAL INPATH '/home/datafile.txt' INTO TABLE <table name>;`|Load unix file to hive tables.
`LOAD DATA INPATH '/tmp/datafile.txt' INTO TABLE <table name>;`|Load hdfs file to hive tables.
`hive> ! /bin/echo "Hello World";`|Run unix command in the hive.
`hive> ! pwd;`|Shows current directory.
`hive> source /home/queries.hql;`|Execute hql script.
`SHOW COLUMNS FROM tabelax;`|Show table columns.
#### DATA TYPE
|||
|-|-|
`ARRAY`|[complex types] e.g. array<string>.
`TIMESTAMP`|[date and time] UTC, format: yyyy-mm-dd hh: mm: ss.fffffffff.
`DATE`|[date and time] Format: yyyy-mm-dd.
`STRING`|[characters] Text.
`CHAR`|[characters] Text with fixed length. The maximum length and set at 255.
`BOOLEAN`|[types miscellaneous].
`DECIMAL`|[numeric] Accuracy of 38 digits. user define precision and scale.
`BINARY`|[types miscellaneous].
`MAP`|[complex types] e.g. map<string,int>.
`STRUCT`|[complex types] e.g. struct<field1:string,field2:string,field3:bigint>.
`TINYINT`|[numeric] Integer 1-byte with sign, -128 up to 127.
`SMALLINT`|[numeric] Integer 2-byte with sign, until -32,768 32,767.
`INT`|[numeric] Entire 4-byte with sign, until -2147483648 2147483647.
`FLOAT`|[numeric] 4-byte floating-point number of single precision.
`DOUBLE`|[numeric] 8-byte number of floating point double precision.
`BIGINT`|[numeric] Entire 8-byte with sign. of -9,223,372,036,854,775,808 until 9,223,372,036,854,775,807.
`VARCHAR`|[characters] Text with length specified between 1 and 65355.
`UNIONTYPE`|[complex types] e.g. uniontype<int, double, array<string>.
