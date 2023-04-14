# WebScraping de la Bolsa de Valores de Lima (BVL) <img align="right" src="https://user-images.githubusercontent.com/106767513/230691533-9372e313-a53e-4b37-872f-9e0fed3fb15f.png" width="10%">

Proyecto que consiste en extraer información de la Bolsa de Valores de Lima y almacenarla para su posterior análisis.
Puedes​ revisar la página en la que se trabajó en el siguiente link: https://www.bvl.com.pe/ 

El proyecto consiste de dos secciones: 

**La primera sección consiste en la extracción de los movimientos diarios de las acciones** (puedes revisar más sobre la BVL [acá](https://www.bvl.com.pe/quienes-somos/quienes-somos-bvl/bolsadevaloresdelima)); esta primera sección puede ser útil para una inspección rápida de la Bolsa o también se puede implementar una alerta cuando alguna acción alcance cierto precio (algo que queda pendiente en el proyecto por el momento).

**La segunda sección consiste en extraer los Estados Financieros** (Estado de Situación Financiera, Estado de Ganancias y Pérdidas, y el Estado de Flujos de Efectivo) de la empresa que se elija y de los años que solicite, como ejemplo se eligieron a las empresas [Alicorp S.A.A.](https://www.bvl.com.pe/emisores/detalle?companyCode=21400#informacion-financiera) y [Volcan Compañía Minera S.A.A.](https://www.bvl.com.pe/emisores/detalle?companyCode=64801#informacion-financiera)

## WebScraping movimientos diarios de la Bolsa de Valores de Lima (BVL)

La información que se encuentra en el [link](https://www.bvl.com.pe/mercado/movimientos-diarios), constituye el registro de las variaciones del precio de las acciones de las empresas listadas en  la BVL, y estas se encuentran variando durante el día desde que abre hasta que cierra la bolsa, con ello se puede dar cuenta del comportamiento del mercado, una información de gran importancia para los que invierten en la Bolsa y buscan rentabilidades. Por ello, considero útil el tener un medio con el cual se pueda tener un acceso más rápido a tal información y de acuerdo a los intereses de cada uno. Una vez extraída la información, podemos  echar un vistazo preliminar de los movimientos de la Bolsa en el siguiente gráfico: 

![figura](https://user-images.githubusercontent.com/106767513/230802046-2a88c122-94a0-4e17-8584-7ba4646c816c.png)

Así mismo, para mayor detalle del código, se muestra un video de la ejecución del mismo, donde se puede apreciar cómo se extrae la información en tiempo real gracias a la librería Selenium de Python:


https://user-images.githubusercontent.com/106767513/231221054-af8d0a77-5818-4d12-b3ed-e5f1e1f7b9b4.mp4


## WebScraping de los Estados Financieros de las empresas que cotizan en la BVL

En esta sección del código se extraen los Estados Financieros(EF) de las empresas que cotizan en la bolsa, podemos elegir cualquier empresa, siempre y cuando cuente con un enlace que nos lleve a su información financiera. A modo de ejemplo se eligieron a Alicorp y Volcan, de los cuales se extrajeron los EF anuales de 4 años consecutivos, en el código se puede elegir el número de periodos o años que se deseen. Toda esa información pasa a ser guardada en los respectivos excel con el nombre de la empresa y contendrá hojas con el nombre de los EF y su respectivo año. Puede visualizar ese proceso en el siguiente video: 


https://user-images.githubusercontent.com/106767513/232159267-74946e87-c921-4aae-bd8d-efde043e50b4.mp4

