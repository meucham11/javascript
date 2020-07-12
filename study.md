

```javascript
배열.length  배열 원소갯수
```


## 추가
```javascript
배열.push(~); 배열 맨뒤에 추가
배열.unshift 배열 맨앞에 추가
배열.splice(index,howmany,내용)
  배열.splice(index,0,'내용')  howmany=0이면 index자리 내용을 삭제하지않고 삽입 
  배열.splice(index,howmany,'asf','wer','sdaf')
```



## 제거
```javascript
배열.shift();  배열 맨앞 제거
배열.pop();    배열 맨뒤 제거  
```

## 객체
```javascript
var a = {'list1' : 10, 'list2':20}
		var b = {'list1' : {'egoing':10,
		                    'k8805':8,
		                    'show' : function(){alert('hello world');
                			}
                }
        }
        document.write(a['list1'],'\n');
        document.write(b['list1']['egoing'],'\n');
        b['list1']['show']();  // 객체에 함수를 넣을 수 있다는것
        
        
var a = {'list' : {'egoing' :10, 'k8805':8, 'sorialgi':80}
			    ,'show': function(){
						console.log(this.list);   // this 해당 객체
					}		
		}
	    a['show']();
      
      
var a = {'list' : {'egoing' :10, 'k8805':8, 'sorialgi':80}
      ,'show': function(){
        for(var name in this.list){
          console.log(name, this.list[name],12312,14124124);
        }
      }		
}
  a.show();

```


## 모듈
라이브러리의 API를 내것으로 만들기
```javascript
// main 파일
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8"/>
	<script type="text/javascript" src="greeting.js"></script>
	
</head>
<body>

<ul>
	<li>egoing</li>
	<li>graphiite</li>
	<li>leezche</li>
</ul>

# hello world<br />	
<script type="text/javascript">
	
	alert(welcome());

</script>

</body>
</html>


// greeting.js  파일 생성
function welcome(){
		return 'Hello world';
	}
```
