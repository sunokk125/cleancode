# cleancode
## var를 지양하자

```
var name = '이름';
var name = '이름2'; // 에러 없음
console.log(name); // 결과 : 이름2
```

같은 변수명을 써도 에러가 없음

###let로 변경시
```
let name = '이름';
let name = '이름2';// error: Identifier 'name' has already been declared.
let name = '이름3';
```

###let 재할당시 
```
let name = '이름';
console.log(name); // 이름
name = '이름2';
console.log(name); // 이름2
name = '이름3';
console.log(name); // 이름3
```

###const로 재할당시
```
const name = '이름';
console.log(name); // 이름
name = '이름2';
console.log(name); // error: Assignment to constant variable.
name = '이름3';
console.log(name);
```

const를 사용하는 것이 더 안전하다

## function scope & block scope
