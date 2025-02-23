# hodu-proto
protocol buffer submodule for hodu

## how to use
1. Use the command below to add this submodule to your repository

    ```
    git submodule add git@github.com:wafflestudio/hodu-proto.git
    ```

2. When you clone the repository which uses submodule for the first time, use the command below

    ```
    git clone --recurse-submodules git@github.com:wafflestudio/hodu-proto.git
    ```

## how to do against modifying of submodule
1. Add the code below to your main project's github workflow. 
    ```
    jobs:
        build:
            runs-on: ubuntu-latest
            steps:
            - name: Checkout repository
                uses: actions/checkout@v4
                with:
                submodules: true  
    ```



