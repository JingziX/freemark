list指令
<p>We have these animals:
<table border=1>
<tr><th>Name<th>Price
<#list animals as being>
<tr><td>${being.name}<td>${being.price} Euros
</#list>
</table>
<#list animals as being>${being.name}</#list>
name会从给定的animals遍历是在每项中重复，从第一项开始，一个接着一个。在所有重复中，being持有当前的值。这个循环变量仅在于<#list>和
</#list>之间。
