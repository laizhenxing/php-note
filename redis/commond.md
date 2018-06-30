> ## Redis 命令
>
> 1. 启动服务端命令
>
>     redis-server
>
> 2.  启动客户端命令
>
>     redis-cli
>
>     注： 使用 ping 命令检测服务端是否正常运行
>
> 3.  在远程服务器上运行命令
>
>     redis-cli -h host -p port -a password
>
> ### Redis 键命令
>
> * [DEL key](https://www.yiibai.com/redis/keys_del.html)
>
>     此命令删除一个指定键（如果存在）
>
> *  [DUMP key](https://www.yiibai.com/redis/keys_dump.html)
>
>     此命令返回存储在指定键的值的序列化版本
>
> *  [EXISTS key](https://www.yiibai.com/redis/keys_exists.html)
>
>     此命令检查是否存在
>
> * [EXPIRE key seconds](https://www.yiibai.com/redis/keys_expire.html)
>
>     设置键在指定时间秒数之后到期/过期。 
>
> * [EXPIPEAT key timestamp](https://www.yiibai.com/redis/keys_expireat.html)
>
>     设置在指定时间戳之后键到期/过期。（这里的时间时 Unix 时间戳格式）
>
> * [PEXPIRE key milliseconds](https://www.yiibai.com/redis/keys_pexpire.html)
>
>     设置键的到期时间（毫秒）
>
> *  [PREPIPEAT key millisecondstimestamp](https://www.yiibai.com/redis/keys_pexpireat.html)
>
>     以Unix时间戳形式来设置键的到期时间(以毫秒为单位)
>
> *  [KEYS pattern](https://www.yiibai.com/redis/keys_keys.html)
>
>     查找与指定模式匹配的所有键值
>
> *  [MOVE key db](https://www.yiibai.com/redis/keys_move.html)
>
>     将键移动到另一个数据库
>
> *  [PERSIST key](https://www.yiibai.com/redis/keys_persist.html)
>
>     删除指定键的过期时间
>
> * [PTTL key](https://www.yiibai.com/redis/keys_pttl.html)
>
>     获取键的剩余过期时间
>
> * [RANDOMKEY](https://www.yiibai.com/redis/keys_randomkey.html)
>
>     从 Redis 返回一个随机的键
>
> * [RENAME key newkey](https://www.yiibai.com/redis/keys_rename.html)
>
>     更改键的名称
>
> * [RENAMEX key newkey](https://www.yiibai.com/redis/keys_renamenx.html)
>
>     如果新键不存在，重命名键
>
> * [TYPE key](https://www.yiibai.com/redis/keys_type.html)
>
>     返回存储在键中的值的数据类型
>
> ### Redis 字符串
>
> * [SET key value](https://www.yiibai.com/redis/strings_set.html)
>
>    设置指定键的值
>
> * [GET key](https://www.yiibai.com/redis/strings_get.html)
>
>    获取指定键的值
>
> * [GETRANGE key start end](https://www.yiibai.com/redis/strings_getrange.html)
>
>    获取存储在键上的字符串的子字符串
>
> * [GETSET key value](https://www.yiibai.com/redis/strings_getset.html)
>
>    设置键的字符串并返回其旧值
>
> * [GETBIT key offset](https://www.yiibai.com/redis/strings_getbit.html)
>
>    返回在键出存储的字符串值中偏移出的位值
>
> * [MGET key1 [key2...]](https://www.yiibai.com/redis/strings_mget.html)
>
>    获取指定键的值列表，返回数组
>
> * [SETBIT key offset value](https://www.yiibai.com/redis/strings_setbit.html)
>
>    存储在键上的字符串值中设置或清除偏移处的位
>
> * [SETEX key seconds value](https://www.yiibai.com/redis/strings_setex.html)
>
>    使用键和到期时间设置值
>
> * [SETNX key value](https://www.yiibai.com/redis/strings_setnx.html)
>
>     设置键的值，仅当键不存在时
>
> * [SETRANGE key offset value](https://www.yiibai.com/redis/strings_setrange.html)
>
>     在指定偏移出开始的键处覆盖字符串的一部分
>
> * [STRLEN key](https://www.yiibai.com/redis/strings_strlen.html)
>
>     获取存储在键中的值的长度
>
> * [MSET key value [key value...]](https://www.yiibai.com/redis/strings_mset.html)
>
>     为多个键分别设置它们的值
>
> * [MSETNX key value [key value]](https://www.yiibai.com/redis/strings_msetnx.html)
>
>     为多个键分别设置他们的值，仅当键不存在时
>
> * [PSETEX key millisenconds value](https://www.yiibai.com/redis/strings_psetex.html)
>
>     设置键的值和到期时间(以毫秒为单位)
>
> * [INCR key](https://www.yiibai.com/redis/strings_incr.html)
>
>     键键的整数值加1，返回一个整数
>
> * [INCRBY key increment](https://www.yiibai.com/redis/strings_incrby.html)
>
>     将键的整数值按给定的数值增加 （increment 只能为）
>
> * [INCRBYFLOAT key increment](https://www.yiibai.com/redis/strings_incrbyfloat.html)
>
>     将间的浮点数值按给定的数值增加（increment 可以为整数，可以为浮点数）
>
> * [DECR key](https://www.yiibai.com/redis/strings_decr.html)
>
>     将键的整数值减1
>
> * [DECRBY key decrement](https://www.yiibai.com/redis/strings_decrby.html)
>
>     按给定的数值减少键的整数值
>
> * [APPEND key value](https://www.yiibai.com/redis/strings_append.html)
>
>     将指定值附加到键
>
> ### Redis 哈希(hash)
>
> * [HSET key field value](https://www.yiibai.com/redis/hashes_hset.html)
>
>     设置散列字段的字符串（给已存在的键赋值会覆盖原有的值）
>
> * [HDEL key field1 [field2]](https://www.yiibai.com/redis/hashes_hdel.html)
>
>     删除一个或多个哈希字段
>
> * [HGET key field](https://www.yiibai.com/redis/hashes_hget.html)
>
>     获取存储在指定键的哈希字段的值
>
> * [HEXISTS key field](https://www.yiibai.com/redis/hashes_hexists.html)
>
>     判断是否存在散列字段
>
> * [HGETALL key](https://www.yiibai.com/redis/hashes_hgetall.html)
>
>     获取存在指定键的哈希中的所有字段和值
>
> * [HKEYS key](https://www.yiibai.com/redis/hashes_hkeys.html)
>
>     获取哈希中所有的字段
>
> * [HLEN key](https://www.yiibai.com/redis/hashes_hlen.html)
>
>     获取三列中的字段数量
>
> * [HVALS key](https://www.yiibai.com/redis/hashes_hvals.html)
>
>     获取哈希中的所有值
>
> * [HMSET key field1 value1 [field2 value2]](https://www.yiibai.com/redis/hashes_hmset.html)
>
>     为多个哈希字段分别设置它们的值
>
> * [HMGET key field1 [field2]](https://www.yiibai.com/redis/hashes_hmget.html)
>
>     获取所有给定的哈希字段的值
>
> * [HSETNX key field value](https://www.yiibai.com/redis/hashes_hsetnx.html)
>
>     仅当字段不存在时，才设置散列字段的值
>
> * [HINCRBY key field increment](https://www.yiibai.com/redis/hashes_hincrby.html)
>
>     将哈希字段的整数值按给定数字增加
>
> * [HINCRBYFLOAT key field increment](https://www.yiibai.com/redis/hashes_hincrbyfloat.html)
>
>     将哈希字段的浮点数值按给定的数字增加
>
> ### Redis 列表命令
>
> * [LPUSH key value1 [value2]](https://www.yiibai.com/redis/lists_lpush.html)
>
>     将一个值或者多个值添加到列表
>
> * [LPOP key](https://www.yiibai.com/redis/lists_lpop.html)
>
>      删除并获取列表中的第一个元素 
>
> * [LRANGE key start stop](https://www.yiibai.com/redis/lists_lrange.html)
>
>      从列表中获取一系列元素
>
> * [LLEN key](https://www.yiibai.com/redis/lists_llen.html)
>
>      获取列表的长度
>
> * [LPUSHX key value](https://www.yiibai.com/redis/lists_lpushx.html)
>
>      仅当列表存在时，才向列表添加值
>
> * [LSET key index value](https://www.yiibai.com/redis/lists_lset.html)
>
>      通过索引在列表中设置元素的值
>
> * [LRTIM key start stop](https://www.yiibai.com/redis/lists_ltrim.html)
>
>      修剪列表的指定范围
>
> * [LINDEX key index](https://www.yiibai.com/redis/lists_lindex.html)
>
>      通过索引从列表中获取元素
>
> * [LINSERT key BEFORE/AFTER pivot value](https://www.yiibai.com/redis/lists_linsert.html)
>
>      在列表中的另一个元素之前或之后插入元素
>
> * [BLPOP key1 [key2] timeout](https://www.yiibai.com/redis/lists_blpop.html)
>
>      删除并获取列表中的第一个元素，或阻塞， 直到有一个元素可用
>
> * [BRPOP key1 [key2 ] timeout](http://www.yiibai.com/redis/lists_brpop.html)
>
>      删除并获取列表中的最后一个元素，或阻塞，直到有一个元素可用 
>
> * [BRPOPLPUSH source destination timeout](http://www.yiibai.com/redis/lists_brpoplpush.html) 
>
>      从列表中弹出值，将其推送到另一个列表并返回它; 或阻塞，直到一个可用 
>
> * [RPUSH key value1 [value2]](http://www.yiibai.com/redis/lists_rpush.html)  
>
>      将一个值或多个值附加到这个列表
>
> * [RPOP key](http://www.yiibai.com/redis/lists_rpop.html) 
>
>      删除并获取列表中的最后一个元素 
>
> * [RPOPLPUSH source destination](http://www.yiibai.com/redis/lists_rpoplpush.html) 
>
>      删除列表中的最后一个元素，将其附加到另一个列表并返回 
>
> * [RPUSHX key value](http://www.yiibai.com/redis/lists_rpushx.html) 
>
>      仅当列表存在时才将值附加到列表 



