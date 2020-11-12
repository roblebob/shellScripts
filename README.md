# Shell Scripts - TryOuts


- [Greg's Wiki](http://mywiki.wooledge.org/ "http://mywiki.wooledge.org/")
  - [BashPitfalls](http://mywiki.wooledge.org/BashPitfalls "http://mywiki.wooledge.org/BashPitfalls")
  - [BashGuide](http://mywiki.wooledge.org/BashGuide "http://mywiki.wooledge.org/BashGuide")


[bash-hackers](https://wiki.bash-hackers.org/start "https://wiki.bash-hackers.org/start")




<br> <br> <br> <br>

- display current shell interpreter (... its within the SHELL environment variable)
  ```shell
  printenv SHELL
  ```


<br> <br> <br> <br>

- PATH environment
  ```shell
  /home/<user>/.profile
  ```
  ```shell
  /home/<user>/.bash_profile`
  ```

<br> <br> <br> <br>

- current working directory
  ```shell
  pwd
  ```

<br> <br> <br> <br>


-  ___rename___ folder

      ```shell
      mv <old> <new>
      ```

<br> <br> <br> <br>


- __help__
  ```shell
  <command> --help
  ```
  ```shell
  man <command>
  ```

<br> <br> <br> <br>




- executing   &nbsp;   ___command1___  &emsp;  _an pipe its output to the args of_  &emsp; ___command2___ &nbsp;     
   ```shell
   <command1> | <command2>
   ```


- executing   &nbsp;   ___command2___  &emsp;  _if, and only if_  &emsp; ___command1___ &nbsp; succeeds    
  ```shell
  <command1> && <command2>
  ```


<br> <br> <br> <br>

- create file
  ```shell
  touch <filename>
  ```



<br> <br> <br> <br>

- display the type of a file
    ```shell
  file <filename>
    ```

<br> <br> <br> <br>



- ___shebang___  = "Hash" + "Bang"
  ```shell
  !/bin/<shell>
  ```


<br> <br> <br> <br>


- __command substitution__
  ```shell
  VAR=$(command)
  ```


  <br> <br> <br> <br>

- __built-ins__
![Alt-Text](https://devconnected.com/wp-content/uploads/2019/12/built-in.png)



  <br> <br> <br> <br>

- change permission
  ```shell
  chmod u+x <script>
  ```
  ⤳ execute script
  ```shell
  ./<script>
  ```


  <br> <br> <br> <br>



- _checking_ if the __user__ is ___root___   &emsp; `USERID=$(id -u)`

    `id -u`  &emsp; &emsp; ⤳ 1000

    `sudo id -u`  &emsp; ⤳ 0




    <br> <br> <br> <br>



- __condition__
  ```shell
  if [[ condition ]]
  then
    command1
  else
    command2
  fi
  ```
