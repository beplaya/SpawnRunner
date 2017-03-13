# SpawnRunner

#### https://github.com/beplaya/SpawnRunner

```
var SpawnRunner = require("spawn_runner");
var runner = new SpawnRunner(debug);//debug ? logs command : silent
runner.run(cmd, cmdArgsArray, function(stdoutString){
    console.log(stdoutString);
});
runner.runInherit(cmd, cmdArgs, function(){
    console.log("done!");
});
```

E.G.
```
runner.run("git", ["branch", "-l"], function(stdoutString){
    console.log(stdoutString);
    // 
    //* develop
    //  master
    //
});

```