## Getting Started

---


1. Get dependencies from npm

  ```bash
  npm install
  ```

2. Run and preview at local (web)

  ```bash
  npm run start:renderer

3. Run and preview at local (electron)

  ```bash
  npm run start:main
  ```

4. Build (web)

  ```bash
  npm run build:renderer
  ```

5. Build (electron)

    you need update `utils/open_im_sdk_wasm/api/database/instance.js` wasm import path first.

    ```javascript
    - SQL = await initSqlJs({ locateFile: () => '/sql-wasm.wasm' });
    + SQL = await initSqlJs({ locateFile: () => '../../sql-wasm.wasm' });
    ```

  ```bash
  npm run build:main
  ```

 

