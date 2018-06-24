> ## Redis 命令
>
> 1. 启动服务端命令
>
>    redis-server
>
> 2.  启动客户端命令
>
>    redis-cli
>
>    注： 使用 ping 命令检测服务端是否正常运行
>
> 3.  在远程服务器上运行命令
>
>    redis-cli -h host -p port -a password
>
> ### Redis 键命令
>
> * [DEL key](https://www.yiibai.com/redis/keys_del.html)
>
>   此命令删除一个指定键（如果存在）
>
> *  [DUMP key](https://www.yiibai.com/redis/keys_dump.html)
>
>   此命令返回存储在指定键的值的序列化版本
>
> *  [EXISTS key](https://www.yiibai.com/redis/keys_exists.html)
>
>   此命令检查是否存在
>
> * [EXPIRE key seconds](https://www.yiibai.com/redis/keys_expire.html)
>
>   设置键在指定时间秒数之后到期/过期。 
>
> * [EXPIPEAT key timestamp](https://www.yiibai.com/redis/keys_expireat.html)
>
>   设置在指定时间戳之后键到期/过期。（这里的时间时 Unix 时间戳格式）
>
> * [PEXPIRE key milliseconds](https://www.yiibai.com/redis/keys_pexpire.html)
>
>   设置键的到期时间（毫秒）
>
> *  [PREPIPEAT key millisecondstimestamp](https://www.yiibai.com/redis/keys_pexpireat.html)
>
>   以Unix时间戳形式来设置键的到期时间(以毫秒为单位)
>
> *  [KEYS pattern](https://www.yiibai.com/redis/keys_keys.html)
>
>   查找与指定模式匹配的所有键值
>
> *  [MOVE key db])(https://www.yiibai.com/redis/keys_move.html)
>
>   将键移动到另一个数据库
>
> *  [PERSIST key](https://www.yiibai.com/redis/keys_persist.html)
>
>   删除指定键的过期时间
>
> * [PTTL key](https://www.yiibai.com/redis/keys_pttl.html)
>
>   获取键的剩余过期时间
>
> * [RANDOMKEY](https://www.yiibai.com/redis/keys_randomkey.html)
>
>   从 Redis 返回一个随机的键
>
> * [RENAME key newkey](https://www.yiibai.com/redis/keys_rename.html)
>
>   更改键的名称
>
> * [RENAMEX key newkey](https://www.yiibai.com/redis/keys_renamenx.html)
>
>   如果新键不存在，重命名键
>
> * [TYPE key](https://www.yiibai.com/redis/keys_type.html)
>
>   返回存储在键中的值的数据类型



