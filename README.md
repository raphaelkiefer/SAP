# SAP
ABAP - Exemplos de Reports 

*&---------------------------------------------------------------------*
*& Report  Z_EMPLOYEE_LIST_01
*&
*&---------------------------------------------------------------------*
*&
*&
*&---------------------------------------------------------------------*

REPORT Z_EMPLOYEE_LIST_01 LINE-SIZE 132.

*INLCUINDO TABELA NO PROGRAMA*
TABLES zEMPLYEES.

*MOSTRANDO TIPOS DE CONFIGURAÇÕES DE LAYOUT DE INFORMAÇÕES
************************
SELECT * FROM zEMPLYEES.
  WRITE zEMPLYEES.
ENDSELECT.

ULINE. -> Underline na tela

SELECT * FROM zEMPLYEES.
  WRITE / zEMPLYEES. 
ENDSELECT.

ULINE.

SELECT * FROM zEMPLYEES.
  WRITE zEMPLYEES.
  WRITE /. -> Quebra de linha na tela
ENDSELECT.

ULINE.

SKIP 2. -> Qubra de linha, com distancia igual a 2 
SELECT * FROM zEMPLYEES.
  WRITE zEMPLYEES.
  WRITE /.
ENDSELECT.
