
<html lang="en-US">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="theme-color" content="#157878">
    <link rel="stylesheet" href="/assets/css/style.css?v=e27bf585b9c641a881074e09853cb11204774c97">
  </head>
  <body>


<h2>Contents</h2>
<ol>
  <li><a href="#samples-seen">V2 和 V3 对比</a></li>

</ol>

<h2>V2 和 V3 对比<a name="samples-seen"></a></h2>
<h3> 只使用第一期数据 </h3>
<h4> 文本</h4>

<table>
    <tr>
      <th style="text-align: left">Speakers</th>
      <td style="text-align: left">V2</td>
      <td style="text-align: left">V3</td>
    </tr>
  
    <tr>
      <th style="text-align: left"><strong>una</strong></th>
      <td style="text-align: left"><audio src="wavs\V2-0626\una.wav" controls="" preload=""></audio></td>
      <td style="text-align: left"><audio src="wavs\V3-0626\v3mix_una_kouyu.mp3" controls="" preload=""></audio></td>
    </tr>

    <tr>
      <th style="text-align: left"><strong>chenqingxin</strong></th>
      <td style="text-align: left"><audio src="wavs\V2-0626\chenqingxin.wav" controls="" preload=""></audio></td>
      <td style="text-align: left"><audio src="wavs\V3-0626\v3mix_chenqingxin_kouyu.mp3" controls="" preload=""></audio></td>
    </tr>
  
</table>


<table>
            <thead>

                <tr>

                    <th>姓名</th>

                    <th>语言</th>

                    <th>分数</th>

                    <th>操作</th>

                </tr>

            </thead>

            <tbody></tbody>

        </table>

   <script>

       

       

        var stus = [{ //假数据

            name: '小明',

            class: 'JavaScript',

            score: 100

        }, {

            name: '小红',

            class: 'JavaScript',

            score: 98

        }, {

            name: '小白',

            class: 'JavaScript',

            score: 89

        }, {

            name: '小石',

            class: 'JavaScript',

            score: 85

        }, {

            name: '小石',

            class: 'JavaScript',

            score: 85

        }];

       

        //数据写入

        var tbody = document.querySelector('tbody'); //找到tbody标签

        for (var i = 0; i < stus.length; i++) { //对stus进行循环遍历，并建立tr标签

            var tr = document.createElement('tr');

            tbody.appendChild(tr);

            for (var k in stus[i]) { //对假数据进行遍历

                var td = document.createElement('td'); //新建td

                td.innerHTML = stus[i][k]; //将对象数据写进td中

                tr.appendChild(td);

            }

            //删除按钮的建立  

            var td = document.createElement('td');

            td.innerHTML = '删除';

            td.className = 'del'

            tr.appendChild(td);

        }

       

       

        //对'删除'进行点击事件    

        var delClick = document.getElementsByClassName('del');

        for (var i = 0; i < delClick.length; i++) {

            delClick[i].onclick = function () {

                tbody.removeChild(this.parentNode);    

            }

    



    
    

  </body>
</html>


