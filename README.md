
more detail http://xingqiba.sinaapp.com

##php.ini
```
wcx.debug = 0
wcx.task_enabled = 0
wcx.task_queue_key = wcx_task_queue
wcx.task_data_key = wcx_task_data
wcx.task_process_interval = 1
```

##functions
```
string wcx_encrypt(to_encrypt_string, to_encrypt_key)
array  wcx_decrypt(to_decrypt_string, to_encrtpt_key)
array  wcx_array_rand(to_rand_array,num)
bool   wcx_bet(rate_num)
void   wcx_lock()
void   wcx_unlock()
array  wcx_task_info()
string wcx_task_post($task, $expect_task_process_timestamp = 0, $task_uuid = '')
bool   wcx_task_delete($task_uuid)
bool   wcx_task_clear()
```

###class
```
$wcx_task_handle = new WcxTask();
$wcx_task_handle->process(function($task){
    //task process
});
$wcx_task_handle->run();
```
