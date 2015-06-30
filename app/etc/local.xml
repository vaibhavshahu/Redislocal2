 <session_save>db</session_save>
        <redis_session>                       <!-- All options seen here are the defaults -->
            <host>127.0.0.1</host>            <!-- Specify an absolute path if using a unix socket -->
            <port>6379</port>
            <password></password>             <!-- Specify if your Redis server requires authentication -->
            <timeout>2.5</timeout>            <!-- This is the Redis connection timeout, not the locking timeout -->
            <persistent></persistent>         <!-- Specify unique string to enable persistent connections. E.g.: sess-db0; bugs with phpredis and php-fpm are known: https://github.com/nicolasff/phpredis/issues/70 -->
            <db>0</db>                        <!-- Redis database number; protection from accidental loss is improved by using a unique DB number for sessions -->
            <compression_threshold>2048</compression_threshold>  <!-- Set to 0 to disable compression (recommended when suhosin.session.encrypt=on); known bug with strings over 64k: https://github.com/colinmollenhour/Cm_Cache_Backend_Redis/issues/18 -->
            <compression_lib>gzip</compression_lib>              <!-- gzip, lzf or snappy -->
            <log_level>1</log_level>               <!-- 0 (emergency: system is unusable), 4 (warning; additional information, recommended), 5 (notice: normal but significant condition), 6 (info: informational messages), 7 (debug: the most information for development/testing) -->
            <max_concurrency>6</max_concurrency>                 <!-- maximum number of processes that can wait for a lock on one session; for large production clusters, set this to at least 10% of the number of PHP processes -->
            <break_after_frontend>5</break_after_frontend>       <!-- seconds to wait for a session lock in the frontend; not as critical as admin -->
            <break_after_adminhtml>30</break_after_adminhtml>
            <bot_lifetime>7200</bot_lifetime>                    <!-- Bots get shorter session lifetimes. 0 to disable -->
        </redis_session>
