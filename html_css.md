## HTML & CSS 学习
---
* ## ***HTML 学习*** 
<a name="first"></a>

### 1. HTML 的概念 & 三大基石 & 标准文档结构
* **概念**
   1. 概念:超文本标记语言
   2. 作用:在浏览器中将数据以友好的方式展现给用户（数据格式化展示）

* **三大基石**
   1. URL （统一资源定位符）
   2. HTML（超文本标记语言）
   3. HTTP（超文本传输协议）

* **标准文档结构**
   ```
   <html>
      <head>
         ...
      </head>
      ......
      <body>
         ...
      </body>
   </html>      
   ```
<a name="second"></a>

### 2. head 标签
   * **title 标签（网页标题）**

   * **meta 标签**
      1. 编码格式设置
         * html 5
         ` <meta charset="utf-8"/> `
         * html 4 
         ` <meta http-equiv="content-type" content="text/html;charset=utf-8"/> `
      2. 提高网页被搜索到的概率
         * 关键字
         ` <meta name="keywords" content="HTML,CSS,前端，学习"/> `   
         * 网页描述
         ` <meta name="description" content="前端学习HTML,CSS的网页。"/> ` 
         * 作者
         ` <meta name="author" content="WeiDustreet"/> ` 
      3. 网页跳转
         * 5 秒自动跳转百度（使用 refresh 报头，可省略“url=”）
         ` <meta http-equiv="refresh" content="5;url=http://www.baidu.com"/> ` 

<a name="third"></a>

### 3. body 标签（文本标签）
   * **标题标签（自动换行，仅有6级标签）**
      1. 代码展示
         ```
         <h1>一级标题</h1>
         <h2>二级标题</h2>
         <h3>三级标题</h3>
         <h4>四级标题</h4>
         <h5>五级标题</h5>
         <h6>六级标题</h6>
         <h7>七级标题</h7> 
         helloworld！ 
         ```
      2. 效果展示
         <h1>一级标题</h1>
         <h2>二级标题</h2>
         <h3>三级标题</h3>
         <h4>四级标题</h4>
         <h5>五级标题</h5>
         <h6>六级标题</h6>
         <h7>七级标题</h7>
         helloworld！
   * **水平线（hr）**
      1. 宽度（width 像素或百分比）
      2. 高度（size 像素）
   * **段落（p 自动换行，段落间距更大）**
   * **换行（br 间距小）**
   * **空格**
   * **权重标签**
      1. 加粗
         * 代码展示
         ` <p>hello<b>world！</b></p> `
         * 效果展示
         <p>hello<b>world！</b></p>         
      2. 斜体
         * 代码展示
         ` <p>hello<i>world！</i></p> `
         * 效果展示
         <p>hello<i>world！</i></p>
      3. 下划线
         * 代码展示
         ` <p>hello<u>world！</u></p> `
         * 效果展示
         <p>hello<u>world！</u></p>
      4. 删除线
         * 代码展示
         ` <p>hello<del>world！</del></p> `
         * 效果展示
         <p>hello<del>world！</del></p>

<a name="fourth"></a>

### 4. body 标签（列表标签）
   * **无序列表**
      * 代码展示
         ```
         <ul>
            <li>北京</li>
            <li>上海</li>
            <li>广州</li>
         </ul>
         ```
      * 效果展示
         <ul>
            <li>北京</li>
            <li>上海</li>
            <li>广州</li>
         </ul>
   * **有序列表**
      1. **无 type 时，默认从 1 开始**
         * 代码展示
            ```
            <ol>
               <li>北京</li>
               <li>上海</li>
               <li>广州</li>
            </ol>
            ```
         * 效果展示
            <ol>
               <li>北京</li>
               <li>上海</li>
               <li>广州</li>
            </ol>
      2. **type="a"**
         * 代码展示
            ```
            <ol type="a">
               <li>北京</li>
               <li>上海</li>
               <li>广州</li>
            </ol>
            ```
         * 效果展示
            <ol type="a">
               <li>北京</li>
               <li>上海</li>
               <li>广州</li>
            </ol>
      3. **type="A"**
         * 代码展示
            ```
            <ol type="A">
               <li>北京</li>
               <li>上海</li>
               <li>广州</li>
            </ol>
            ```
         * 效果展示
            <ol type="A">
               <li>北京</li>
               <li>上海</li>
               <li>广州</li>
            </ol>
      4. **type="i"**
         * 代码展示
            ```
            <ol type="i">
               <li>北京</li>
               <li>上海</li>
               <li>广州</li>
            </ol>
            ```
         * 效果展示
            <ol type="i">
               <li>北京</li>
               <li>上海</li>
               <li>广州</li>
            </ol>
      5. **type="I"**
         * 代码展示
            ```
            <ol type="I">
               <li>北京</li>
               <li>上海</li>
               <li>广州</li>
            </ol>
            ```
         * 效果展示
            <ol type="I">
               <li>北京</li>
               <li>上海</li>
               <li>广州</li>
            </ol>
   * **自定义列表**
      * 代码展示
         ```
         <dl>
            <dt>几个城市：</dt>
            <dd>北京</dd>
            <dd>上海</dd>
            <dd>广州</dd>
         </dl>
         ```
      * 效果展示（不知道为什么会有斜体。。。）
         <dl>
            <dt>几个城市：</dt>
            <dd>北京</dd>
            <dd>上海</dd>
            <dd>广州</dd>
         </dl>

<a name="fifth"></a>

### 5. 图片标签（不自动换行，行内元素）
   * **路径（src）**
      1. 绝对路径
      2. 相对路径

   * **图片大小**
      1. 仅改变宽度或者高度，图片会自动按比例放缩

   * **title（鼠标悬浮在图片上出现的文字）**
   * **alt（图片未能加载出成功时出现的文字）**   

<a name="sixth"></a>

### 6. 超链接标签
   * **路径（href）**
   * **target**
      1. _self（在当前页中刷新显示）
      2. _blank（在新的标签页中显示）
      3. _top（在顶层页面中显示）
      4. _parent（在父级页面中刷新）

   * **锚点**
      * 代码展示
      ```
      <!--
      ----   需要先在每个对应的段落前加上
      ----   <a name="first"></a>
      ----   ...
      -->
      <a href="#first">1. HTML 的概念 & 三大基石 & 标准文档结构</a><br>
      <a href="#second">2. head 标签</a><br>
      <a href="#third">3. body 标签（文本标签）</a><br>
      <a href="#fourth">4. body 标签（列表标签）</a><br>
      <a href="#fifth">5. 图片标签</a><br>
      <a href="#sixth">6. 超链接标签</a><br>
      <a href="#seventh">7. 表格标签</a><br>
      ```
      * 效果展示

         <a href="#first">1. HTML 的概念 & 三大基石 & 标准文档结构</a><br>
         <a href="#second">2. head 标签</a><br>
         <a href="#third">3. body 标签（文本标签）</a><br>
         <a href="#fourth">4. body 标签（列表标签）</a><br>
         <a href="#fifth">5. 图片标签</a><br>
         <a href="#sixth">6. 超链接标签</a><br>
         <a href="#seventh">7. 表格标签</a><br>


<a name="seventh"></a>

### 7. 表格标签



### 8. 内嵌标签
   * **iframe 标签**

      1. 单个页面
         * 代码展示
         ` <iframe src="http://www.baidu.com" width="50%" height="200px"> `

         * 效果展示
         <iframe src="http://www.baidu.com" width="100%" height="200px">

      2. 多页面
         * 代码展示
         ```
         <a href="http://www.baidu.com" target="baidu">百度一下</a>
         <a href="http://www.sou.com" target="360sou">360搜索</a><br>
         <iframe src="" width="50%" height="400px" name="baidu"></iframe>
         <iframe src="" width="50%" height="400px" name="360sou"></iframe>
         ```

         * 效果展示
         <a href="http://www.baidu.com" target="baidu">百度一下</a>
         <a href="http://www.sou.com" target="baidu">360搜索</a><br>
         <iframe src="" width="50%" height="400px" name="baidu"></iframe>
         <iframe src="" width="50%" height="400px" name="360sou"></iframe>





