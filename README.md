# sqlite3_exec_stmt
One-Step Query Execution Interface with statement for sqlite3

Copyright (c) 2007-2015 Ing-Long Eric Kuo

Distributed under the MIT License.
http://opensource.org/licenses/MIT

## Example usage
```
sqlite3_stmt *select;
sqlite3_prepare_v2(db, selectsql.c_str(), selectsql.length(), &select, NULL);		
sqlite3_exec_stmt(select, &my_callback, this, NULL);
sqlite3_finalize(select);	
```