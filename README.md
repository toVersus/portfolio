## Usage

1. Cloning the repository

    ```
    $ git clone https://toversus@bitbucket.org/toversus/portfolio.git
    $ cd ./portfolio
    $ npm install
    ```

2. Serving up my portfolio with GitHub-like css format

    ```
    $ ./node_modules/.bin/http-server
    ```

3. Updating the contents

4. Converting html to pdf

    ```
    $ wkhtmltopdf http://127.0.0.1:8080/ portfolio.pdf
    ```

5. Encrypting pdf file

    ```
    $ USER_PASSWD="M+F0hWBR57DHN6HTYG6HoikiuyxRTNC1I0wz/6a/EC8="
    $ OWNER_PASSWD="pl/vt/vffPwUaIcByWmJeJTSsjW4FRueQepS54kpzIA="
    $ qpdf  --encrypt $USER_PASSWD $OWNER_PASSWD 40 --print=n --modify=n --extract=n --annotate=n -- portfolio.pdf encrypted-portfolio.pdf
    ```
