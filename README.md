AddressData(Taiwan)
======================

The original data is provided by Chunghwa Post Co., Ltd.

---
A snippet of original data
<br><i><u>last update: 2015/05/07  official ver.10403</u></i>
<pre><code>
10058臺北市中正區  八德路１段              全                            
10079臺北市中正區  三元街                  單全                          
10070臺北市中正區  三元街                  雙  48號以下                  
10079臺北市中正區  三元街                  雙  50號以上                  
10068臺北市中正區  大埔街                  單  15號以上                  
10068臺北市中正區  大埔街                  雙  36號以上                  
10051臺北市中正區  中山北路１段            單   3號以下                  
10041臺北市中正區  中山北路１段            雙  48號以下           
...               
</code></pre>
A snippet of address_data.sql where any street name contains "１、２、３．．．"　
<br>the chars are replaced by "一、二、三"
and "台" are replaced by "臺"
<br><i><u>last update: 2014/12/25</u></i>
<pre><code>
...
INSERT INTO `address_name` (`uid`, `name`, `link`) VALUES
(1, '臺北市', 0),
(2, '中正區', 1),
(3, '八德路一段', 2),
(4, '三元街', 2),
(5, '大埔街', 2),
(6, '中山北路一段', 2),           
...               
</code></pre>
Here's how the corresponding table look like

<table>
	<tr>
		<th>id</th>
		<th>name</th>
		<th>link</th>
	</tr>
	<tr>
		<td>1</td>
		<td>臺北市</td>
		<td>0</td>
	</tr>
	<tr>
		<td>2</td>
		<td>中正區</td>
		<td>1</td>
	</tr>
	<tr>
		<td>3</td>
		<td>八德路一段</td>
		<td>2</td>
	</tr>
</table>