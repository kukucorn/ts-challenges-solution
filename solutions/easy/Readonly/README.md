```ts
type MyReadonly<T> = { readonly [key in keyof T]: T[key]};
```
제시된 테스트 케이스는 통과되는데, 프로퍼티의 depth가 2 이상일 때는 readonly가 선언되지 않는다.  
연관된 문제로 Medium 난이도에 [DeepReadonly](https://github.com/type-challenges/type-challenges/blob/master/questions/9-medium-deep-readonly/README.md)가 있다.