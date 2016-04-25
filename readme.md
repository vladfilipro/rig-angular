# rig-angular
A rig containing a task used for outputting messages to console

## How to use
1. Install rigs package: `npm install rigs`
2. Install rig-angular: `npm install rig-angular`

## Available tasks in rig-angular
- `rig-angular__output`: A task which outputs the configured message to the console
  - properties:
    - `message`: String, contains the message to be displayed

    ```
    {
        taskname: 'rig-angular__output',
        dependency: [],
        message: 'This is an example'
    }
    ```

### Generated using [webcase-rig](https://www.npmjs.com/package/webcase-rig) version 1.0.1
