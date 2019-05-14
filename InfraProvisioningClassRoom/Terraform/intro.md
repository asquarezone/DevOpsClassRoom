# Terraform

## Building Blocks
* __Provider__: 
    * Where the environmnet has to be created
    * It also has way to connect to environment
    * Defines type of provider & connection argumenteters
    * Syntax:
    ```
    provider <type>
    {
        <argument1> = <value1>
        ..
        ..
        ..
        <argumentn> = <valuen>
    }
    ```
    * Example
    ```
    provider 'aws' {
        access_key =
        secret_key =
        region = 
    }
    ```

* __Resource__:
    * What is that you want to create
    * Every Provider has set of supported resources
    * Syntax:
    ```
    resource '<type>', '<name>' {
        <argument1> = <value1>
        ..
        ..
        ..
        <argumentn> = <valuen>
    }
    ```
