# yarn 2 Workspaces bug

Run `make bug` to see the issue.

On a non-M1 Mac you will see:

```
➜  test-yarn-2-bug git:(main) make bug
yarn install
➤ YN0000: ┌ Resolution step
➤ YN0000: └ Completed
➤ YN0000: ┌ Fetch step
➤ YN0000: └ Completed
➤ YN0000: ┌ Link step
➤ YN0000: └ Completed
➤ YN0000: Done in 0s 17ms
yarn workspaces foreach -v run build
➤ YN0000: [a]: a
➤ YN0000: [b]: b
```

On an M1 Mac you will see:

```
➜  test-yarn-2-bug git:(main) make bug
yarn install
➤ YN0000: ┌ Resolution step
➤ YN0000: └ Completed
➤ YN0000: ┌ Fetch step
➤ YN0000: └ Completed
➤ YN0000: ┌ Link step
➤ YN0000: └ Completed
➤ YN0000: Done in 0s 17ms
yarn workspaces foreach -v run build
➤ YN0000: [a]: a
```
