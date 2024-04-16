# WebScript-Speedtest
Apache, Nginx (OpenResty), IIS, 
PHP, Lua, NodeJs, Speedtest

Performance test : 

-n requests
-c concurrency

/Apache/bin/

ab -n 100 -c 1 http://localhost:8080/

ab -n 10000 -c 1 http://localhost:8080/

ab -n 10000 -c 100 http://localhost:8080/

ab -n 10000 -c 1000 http://localhost:8080/

ab -n 10000 -c 10000 http://localhost:8080/

** run 3 to 5 test and select the middle speed.

Test 1. fixed html / show random number.

Test 2. Load static html file and display.

Test 3. connect to db and do a simple query, response result.

    node.js : Error: ER_CON_COUNT_ERROR: Too many connections
