# NodeJs-Speedtest
NodeJs and PHP Speedtest

Performance test : 

http://localhost:8080/

http://localhost/LoadTest/Php01.php

-n requests
-c concurrency

/Apache/bin/

ab -n 10000 -c 1 http://localhost:8080/
ab -n 10000 -c 100 http://localhost:8080/
ab -n 10000 -c 1000 http://localhost:8080/
ab -n 10000 -c 10000 http://localhost:8080/

ab -n 10000 -c 1 http://localhost/LoadTest/php/Php01.php
ab -n 10000 -c 100 http://localhost/LoadTest/php/Php01.php
ab -n 10000 -c 1000 http://localhost/LoadTest/php/Php01.php
ab -n 10000 -c 10000 http://localhost/LoadTest/php/Php01.php

ab -n 10000 -c 1 http://localhost/LoadTest/php/Php02.php
ab -n 10000 -c 100 http://localhost/LoadTest/php/Php02.php
ab -n 10000 -c 1000 http://localhost/LoadTest/php/Php02.php
ab -n 10000 -c 10000 http://localhost/LoadTest/php/Php02.php

ab -n 10000 -c 1 http://localhost/LoadTest/php/Php03.php
ab -n 10000 -c 100 http://localhost/LoadTest/php/Php03.php
ab -n 10000 -c 1000 http://localhost/LoadTest/php/Php03.php
ab -n 10000 -c 10000 http://localhost/LoadTest/php/Php03.php



** run 3 test and select fastest.

1. no database connection.
2. Load static html file and reply.
3. connect to db and do a simple query, response result.

    node.js : Error: ER_CON_COUNT_ERROR: Too many connections
