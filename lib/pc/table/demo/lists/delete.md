# 删除

`del` 参数可以指定行删除操作,参数有:

- `url`: 提交的url
- `method`: 方法类型
- `beforeSend`: 提交之前操作,返回值为提交时的参数.第一个参数为当前行信息
- `success`: 请求成功后回调,返回对象中,`ok`是`bool`表示是否成功,`message`是`string`表示错误时的提示,第一个参数为返回值内容
- `alert`: 回调,返回值是点击删除按钮后弹出的提示,第一个参数是列信息

删除成功后,如果当前页剩余条目只有一个,且不是第一页,刷新到上一页,否则刷新当前页面