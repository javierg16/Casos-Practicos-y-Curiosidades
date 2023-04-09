# WebScraping de la Bolsa de Valores de Lima (BVL<img align="left" src="https://user-images.githubusercontent.com/106767513/230691533-9372e313-a53e-4b37-872f-9e0fed3fb15f.png" width="10%">) <img align="right" src="https://user-images.githubusercontent.com/106767513/230691533-9372e313-a53e-4b37-872f-9e0fed3fb15f.png" width="10%">

Proyecto que consiste en extraer información de la Bolsa de Valores de Lima y almacenarla para su posterior análisis.
Puedes​ revisar la página en la que se trabajó en el siguiente link: https://www.bvl.com.pe/ 

El proyecto consiste de dos secciones: 

**La primera sección consiste en la extracción de los movimientos diarios de las acciones** (puedes revisar más sobre la BVL [acá](https://www.bvl.com.pe/quienes-somos/quienes-somos-bvl/bolsadevaloresdelima)); esta primera sección puede ser útil para una inspección rápida de la Bolsa o también se puede implementar una alerta cuando alguna acción alcance cierto precio (algo que queda pendiente en el proyecto por el momento).

**La segunda sección consiste en extraer los Estados Financieros** (Estado de Situación Financiera, Estado de Ganancias y Pérdidas, y el Estado de Flujos de Efectivo) de la empresa que se elija y de los años que solicite, como ejemplo se eligieron a las empresas [Alicorp S.A.A.](https://www.bvl.com.pe/emisores/detalle?companyCode=21400#informacion-financiera) y [Volcan Compañía Minera S.A.A.](https://www.bvl.com.pe/emisores/detalle?companyCode=64801#informacion-financiera)

## WebScraping movimientos diarios de la Bolsa de Valores de Lima (BVL)

La información que se encuentra en el [link](https://www.bvl.com.pe/mercado/movimientos-diarios), constituye el registro de las variaciones del precio de las acciones de las empresas listadas en  la BVL, y estas se encuentran variando durante el día desde que abre hasta que cierra la bolsa, con ello se puede dar cuenta del comportamiento del mercado, una información de gran importancia para los que invierten en la Bolsa y buscan rentabilidades. Por ello, considero útil el tener un medio con el cual se pueda tener un acceso más rápido a tal información y de acuerdo a los intereses de cada uno. Una vez extraída la información, podemos  echar un vistazo preliminar de los movimientos de la Bolsa en el siguiente gráfico: 

<iframe src="mi_grafico.html"></iframe>
