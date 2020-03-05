# Javascript 연습문제
## 로그인창 만들기
```
<!DOCTYPE html>
<html>

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
  <style media="screen">
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    ul {
      width: 400px;
      margin: 0 auto;
      list-style: none;
    }
    label{
      display:inline-block;
      width:40px;
    }
    ul li {
      text-align: center;
      margin: 20px 0;
    }
    ul li button {
      width: 100px;
      height:30px;
    }

    ul li button:last-child {
      margin-left: 30px;
    }
  </style>
</head>

<body>
  <ul>
    <li><label for="id">ID :</label> <input type="text" id="id"></li>
    <li><label for="pw">PW :</label> <input type="password" id="pw"></li>
    <li> <button id='btn'>확인</button><button>취소</button> </li>
  </ul>
  <script type="text/javascript">
    var btn=document.getElementById('btn');
    var txtId=document.getElementById('id');
    btn.addEventListener('click',function(){
      if(txtId.value==""){
        alert('id입력하세요.');
      }else{
        alert(txtId.value+"님 반갑습니다!");
      }
    });
  </script>
</body>

</html>
```
