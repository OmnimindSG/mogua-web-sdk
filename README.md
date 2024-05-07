
## Installation 

To install the MoguaSDK package, use the following command:

```bash
npm install moguasdk
```

## Importing the Package

You can import the MoguaSDK package into your JavaScript file using the require function:

[//]: # (language="JSX")
```jsx
const { MoguaSDK } = require('moguasdk');
```
[//]: # (language="TSX")
```tsx
import { MoguaSDK } from "moguasdk";
```

## Use MoguaSDK With UMD build

We also provide a UMD build for sites that don't use npm or modules. The UMD build exports a global MoguaSDK Class. You can import MoguaSDK from **www.mogua.io** in your html code.

```html
<script src="https://www.mogua.io/script/moguasdk/index.umd.js" ></script>
```

## Using the MoguaSDK Class

After importing the MoguaSDK class from the moguasdk package, you can create an instance of the class with the app key of your application. Meanwhile, you can set the parameters which will be sent to your application.

```jsx
const mogua = new MoguaSDK(app_key, parameters);
```

Now, you can use the methods of the MoguaSDK class to get the data in instance:

```jsx
//get customized parameters from sdk instance
mogua.getData();
```

You can use the methods provided by the MoguaSDK class to send Attribution data to the Mogua API. 


```jsx
//register web view user and record a web_view event
mogua.register();
//record a download event
mogua.download(): void;
//record a customized event
mogua.sendEvent(name: string);
```

## Troubleshooting

If you encounter any issues while using the MoguaSDK class from the moguasdk package, please check the following:

- Make sure you have the latest version of the moguasdk package.
- Make sure you have correctly imported the MoguaSDK class from the moguasdk package.
- Look for any error messages in the console.

If the problem persists, please reach out to the moguasdk package's maintainers or check the moguasdk package's documentation for further assistance.