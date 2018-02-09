## 垂直居中的方法

1. 行内元素
```
text-align:center;
line-height: 100px;
height: 100px;
```
2. 块级元素 3种定位方法
  父级元素
  ```
  position: relative;
  height:200px;
  width:100%;
  ```
  子级元素
  2.1
  ```
  position:absolute;
  width:100px;
  height:100px;
  top: 50%;
  left:50%;
  margin-top:-50px;
  margin-left:-50px;
  ```
  2.2
  ```
  position: absolute;
  width:100px;
  height:100px;
  top:50%;
  left:50%;
  transform: translate(-50%, -50%);
  ```
  2.3
  ```
  position:absolute;
  width:100px;
  height:100px;
  top:0;
  left:0;
  bottom:0;
  right:0;
  margin:auto;
  ```
3. 块级元素 display:table-cell
  父级元素
  ```
  display: table;
  width:100%;
  height:200px;
  ```
  子级元素
  ```
  display:table-cell;
  vertical-align:middle;
  text-align:center;
  ```

4. 块级元素 flex
   父级元素
   ```
   display:flex
   align-items: center;
   justify-content: center;
   ```
