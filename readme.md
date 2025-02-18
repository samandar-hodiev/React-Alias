# React - Alias

## `File line view `

![alt text](./images/img1.png)

<hr>
<br><br><br><br><br><br><br><br><br><br><br><br>

## `vite.config.js`

![alt text](./images/img2.png)

<br><br>

    import { defineConfig } from 'vite'
    import path from 'path'
    import react from '@vitejs/plugin-react'



    export default defineConfig({
         plugins: [react()],
      resolve:{
        alias:{
         "@":path.resolve(__dirname, "./src"),
         "@images":path.resolve(__dirname, "./src/assets/images"),
         "@icons":path.resolve(__dirname, "./src/assets/icons"),
         "@layouts":path.resolve(__dirname, "./src/components/layouts"),
         "@ui":path.resolve(__dirname, "./src/components/ui"),
         "@sections":path.resolve(__dirname, "./src/components/layouts/sections"),
         "@form":path.resolve(__dirname, "./src/components/form"),
         "@mainLayout":path.resolve(__dirname, "./src/main-lyouts"),
         "@components":path.resolve(__dirname, "./src/components"),
         "@mocks":path.resolve(__dirname, "./src/mocks"),
         "@pages": path.resolve(__dirname, "./src/pages"),
        "@router":path.resolve(__dirname, "./src/router"),
       }
      }
    })

<hr>
<br><br><br><br><br><br><br><br><br>


## `jsconfig.json`

![alt text](./images/img3.png)

<br><br>



    {
       "compilerOptions": {
          "paths": {
            "@/*":["./src/*"],
            "@images/*":["./src/assets/images/*"],
            "@icons/*":["/src/assets/icons/*"],
            "@layouts/*":["./src/components/layouts/*"],
            "@ui/*":["./src/components/ui/*"],
            "@sections/*":["./src/components/layouts/sections/*"],
            "@form/*":["./src/components/form/*"],
            "@mainLayout/*":["./src/main-lyouts/*"],
            "@components/*":["./src/components/*"],
            "@mocks/*":["./src/mocks/*"],
            "@pages/*":["./src/pages/*"],
            "@router/*":["./src/router/*"],
        }
      }
    }


