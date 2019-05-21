# Debug Node.js Apps in Docker Container using VSCode

1. Build Image

```
docker build -t tmp/sample-nodejs . 
```

2. Run

```
docker run -it -p 3000:3000 -p 9229:9229 -v $(pwd)/src:/workspace tmp/sample-nodejs npm run dev
```

3. Debug

Exec "Docker: Attach to Node" in VSCode Debug Tab

4. Enjoy Debugging
