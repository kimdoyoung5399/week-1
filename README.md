# ๐ถ ๋์ ์ฒซ TodoList

---

ํญํด 99 3์ฃผ์ฐจ React ์๋ฌธ์ฃผ์ฐจ ๊ฐ์ธ๊ณผ์ ์ ์ฒ์์ผ๋ก React๋ก ๋ง๋ค์ด ๋ณด์๋ค.

![initial](https://user-images.githubusercontent.com/112137813/193992953-9445191f-e68b-40ce-b844-28e4d0bc14b7.png)

---

### ๐๊ตฌํ๊ธฐ๋ฅ

1. Todo ์ถ๊ฐํ๊ธฐ

* ์ ๋ชฉ๊ณผ ๋ด์ฉ์ ์๋ ฅํ๊ณ  ์ถ๊ฐํ๊ธฐ ๋๋ฅด๋ฉด Working.. ๐ฅ ์๋์ ์๋ก์ด Todo ์์ฑํ input ์๋ ฅ์ฐฝ ์ด๊ธฐํ

2. Todo ์ํ์ ๋ฐ๋ฅธ ์์น ๋ฐฐ์น

* Todo๋ฅผ ์๋ฃํ๊ธฐ ์ ์ด๋ฉด Working.. ๐ฅ ๋ผ์ธ, Done..! ๐ ๋ผ์ธ์ ์๊ธฐ๋ฉฐ, ์ทจ์, ์๋ฃ์ ๋ฐ๋ฅธ ์ํ ๋ณํ
* ์ญ์ ํ๊ธฐ ๋ฒํผ ๋๋ฅด๋ฉด TodoList์์ ์ญ์ 

---

### ๐Trouble Shooting

1. ํ์ผ import ํ ๋ vscolde์์ ์๋์์ฑ์ผ๋ก ์๋ ฅ์ ๋์๋ฌธ์ ๊ตฌ๋ณ๋ชปํด์ ์๋ฌ ๋ฐ์
   *  ๋์๋ฌธ์ ์๋ ฅ ํ์ธ ํ์!

```
Failed to compile.

Module not found: Error: Cannot find file: 'Todolist.jsx' does not match the corresponding name on disk: './src/pages/TodoList.jsx'.
ERROR in ./src/components/layout/Layout.jsx 7:0-44
Module not found: Error: Cannot find file: 'Todolist.jsx' does not match the corresponding name on disk: './src/pages/TodoList.jsx'.

webpack compiled with 1 error
```

2. button ์ฌ์ฉํ์ฌ ์ถ๊ฐํ๊ธฐ ๋ฒํผ ๋๋ฅด๋ฉด ์ถ๊ฐ์ฆ์ ์๋ก๊ณ ์นจ..

  * form ํ๊ทธ์์ button ํ๊ทธ ์ฌ์ฉ์ tpye ํ์ธ!!

3. A component is changing an uncontrolled input to be controlled.

  * ์ธํ์ฐฝ์ ์๋ ฅํ๋ ์๊ฐ ์ด๋ฐ ์๋ฌ๊ฐ ๋จ๋๋ผ.. input value ๋ก undefined ๊ฐ ๋ค์ด๊ฐ๋ค๊ณ  ์๋ฌ๋ฉ์ธ์ง๋ฅผ ๋์ด๊ฒ์ด๋ค..

  * Form ํ๊ทธ ์์ key : value ์ ์ด๋ฆ ๋๋ ๋์๋ฌธ์ ํ์ธ... ๋๊ตฌ์๊ฒ ์ค๋ชํ๋ค๊ฐ ํ์ธ๋์ด ๊ณ ์น๋ ์ ์์์์ด ๋๋น!

```
A component is changing an uncontrolled input to be controlled. This is likely caused by the value changing from undefined to a defined value, which should not happen. Decide between using a controlled or uncontrolled input element for the lifetime of the component.
```

---

์ฒ์์ผ๋ก React๋ก ๋ง๋ค์ด ๋ดค๋๋ฐ ์์ง๊น์ง๋ ์ด๋ ต๋ค...
๊ฐ์ฅ ๊ธฐ๋ณธ์ ์ธ state , props ๋ฑ๋ฑ..
๋ฐฐ์ธ๊ฒ ์์ง ๋ง์ง๋ง ์์ผ๋ก ๋ ๋ธ๋ ฅ ํด๋ด์ผ๊ฒ ๋ค.
