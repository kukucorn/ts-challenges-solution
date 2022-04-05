```ts
type MyPick<T, K extends keyof T> = {
  [key in K]: T[key]
}
```

extends를 사용해서 K의 타입을 T의 key로 제한하고,
index signature를 사용해서 K의 타입만을 사용하는 MyPick을 생성한다.