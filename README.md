# learning-typescript
Just for learning typescript...

## Setup the environment

- Install the typescript in global
```
npm i typescript -g
```

- Create the tsconfig file -- tsconfig.json
```
tsc --init
```

- Setup the complier
```
# tsconfig.json
{
    "compilerOptions": {
        "target": "es2016",
        "rootDir": "./src",
        "outDir": "./build/js",
    },
    "include": [
        "src"
    ]
}
```

- Create `src`, `build` directory on the top level directory
```
mkdir {build, src}
touch build/index.html
touch src/main.ts
```

- Starting watching the top level directory for compliering
```
tsc -w
```