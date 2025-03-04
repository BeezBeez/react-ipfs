<div align="center">

# react-ipfs

React IPFS instance hooks for easier usage in your DAPPS


 ![npm](https://img.shields.io/npm/dw/react-ipfs) ![David](https://img.shields.io/david/youaresoroman/react-ipfs) ![GitHub package.json dependency version (prod)](https://img.shields.io/github/package-json/dependency-version/youaresoroman/react-ipfs/ipfs) ![GitHub top language](https://img.shields.io/github/languages/top/youaresoroman/react-ipfs) ![NPM](https://img.shields.io/npm/l/react-ipfs) ![Matrix](https://img.shields.io/matrix/ipfs-awesome:matrix.org?server_fqdn=matrix.org)

 </div>

## Installation

### npm

```bash
npm install react-ipfs
```

### yarn
```bash
yarn add react-ipfs
```
## Documentation
TSDoc compiled documentation is [here](https://youaresoroman.github.io/react-ipfs/)

## Usage

src/index.tsx
```js
import { IPFSProvider } from "react-ipfs"

....
    <IPFSProvider fallback={<>LOADING</>}>
      <App />
    </IPFSProvider>
...
```

src/App.tsx
```js
import { useIPFS } from '@lib';

function App() {
  const ipfs = useIPFS()

  useEffect(()=>{
      ipfs.node.id().then(console.log);
  },[])

...
```
## Contribute

Please see the [contributing guidelines](./CONTRIBUTING.md)
