### unshift
<pre><code>
columns.unshift({ header: "No", name: "autoNumber" , width: "20" , align : "center" , defaultColumn:true, fixed: true})
</code></pre>

끝에 배열 추가 
unshift() 매서드는 새로운 요소를 배열의 맨 앞쪽에 추가

### filter 
filter() 메서드는 주어진 함수의 테스트를 통과하는 모든 요소를 모아 새로운 배열로 반환합니다.
<pre><code>
const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

const result = words.filter(word => word.length > 6);

console.log(result);
// expected output: Array ["exuberant", "destruction", "present"]
</code></pre>

<pre><code>
var defaultColumns = columns.filter(function(elem, idx){
			if(elem.defaultColumn == true){
				return elem
			}
		})
</code></pre>