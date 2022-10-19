# Part1

## variables
1. 20 
2. 20
3. 20
4. `ReferenceError: result is not defined
    at sumValues (C:\Users\xuech\fa22-cse110-lab4\expose\javascript\test.js:11:35)
    at Object.<anonymous> (C:\Users\xuech\fa22-cse110-lab4\expose\javascript\test.js:14:1)
    at Module._compile (node:internal/modules/cjs/loader:1119:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1173:10)
    at Module.load (node:internal/modules/cjs/loader:997:32)
    at Module._load (node:internal/modules/cjs/loader:838:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:81:12)
    at node:internal/main/run_main_module:18:47` 

    This is because `let` variable cannot be accessed outside the block (if condition), thus print statement outside will deem `result` not defined.
5. `        result = num1 + num2;
               ^
TypeError: Assignment to constant variable.
    at sumValues (C:\Users\xuech\fa22-cse110-lab4\expose\javascript\test.js:7:16)
    at Object.<anonymous> (C:\Users\xuech\fa22-cse110-lab4\expose\javascript\test.js:16:1)
    at Module._compile (node:internal/modules/cjs/loader:1119:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1173:10)
    at Module.load (node:internal/modules/cjs/loader:997:32)
    at Module._load (node:internal/modules/cjs/loader:838:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:81:12)
    at node:internal/main/run_main_module:18:47`

    This is because the value assigned to `const` is not mutable, by reassigning new value to `result` caused error. 

6. same error, this is because the value assigned to `const` is not mutable, by reassigning new value to `result` caused error. 
