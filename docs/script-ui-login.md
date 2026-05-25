# Script Robot Framework — Login

```robot
*** Settings ***
Library    SeleniumLibrary

*** Variables ***
${URL}        file:///C:/Users/perei/OneDrive/Área%20de%20Trabalho/InfoMed_teste_de_software-main/InfoMed_teste_de_software-main/index.html
${BROWSER}    chrome

*** Test Cases ***
CT01 - Login válido
    Open Browser    ${URL}    ${BROWSER}
    Maximize Browser Window

    Input Text    xpath=//input[@type='email']    teste@exdex.com
    Input Password    xpath=//input[@type='password']    123456

    Click Button    xpath=//button[contains(text(),'Entrar')]

    Sleep    3s

    Close Browser

CT02 - Login inválido
    Open Browser    ${URL}    ${BROWSER}
    Maximize Browser Window

    Input Text    xpath=//input[@type='email']    errado@erro.com
    Input Password    xpath=//input[@type='password']    111111

    Click Button    xpath=//button[contains(text(),'Entrar')]

    Sleep    3s

    Close Browser
```