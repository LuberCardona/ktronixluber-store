# store-theme ktronixluber-store

Store-theme es una tienda de tecnología y electrodomésticos basada en VTEX IO Store Framework.

## Previsualización
## Vista de Escritorio - Header, Home and Footer
![preview-desktop](https://user-images.githubusercontent.com/66228518/197647662-585714f0-a485-463e-bdfa-7018b653d0f0.png)

## Vista en Tableta - Header, Home and Footer
![preview-tablet](https://user-images.githubusercontent.com/66228518/197648516-42eaa825-8ad0-42b5-b0bd-c1b54ddf35b0.png)

## Vista en Teléfono - Header, Home and Footer
![preview phone](https://user-images.githubusercontent.com/66228518/197649074-37890bef-4832-44ae-9221-fd218e2dcb62.png)

## Vista de Escritorio - Página lista de productos
![PLP-desktop](https://user-images.githubusercontent.com/66228518/197649841-d6e72fcd-9222-4844-92e6-7273b9b5dfe0.JPG)

## Vista en móviles - Página lista de productos
![PLP-phone](https://user-images.githubusercontent.com/66228518/197650262-c05044c6-30a8-408c-9fc3-d22f1b054ee4.JPG)

## Vista de Escritorio - Página detalle de producto
![PDP-desktop](https://user-images.githubusercontent.com/66228518/197650727-1277011d-d8a4-4a92-a672-a76f62e1eb71.JPG)

## Vista en Tableta - Página detalle de producto
![PDP-tablet](https://user-images.githubusercontent.com/66228518/197651048-cd833982-f4c7-4f80-bf8e-93cc2c4490c3.JPG)

## Vista en Teléfono - Página detalle de producto
![PDP-phone](https://user-images.githubusercontent.com/66228518/197651094-72a8e75e-76a3-42ea-bece-cbbe0c615a3e.JPG)

## Vista de Escritorio - Página estática (/quienes-somos)
![quinesSomos-desktop](https://user-images.githubusercontent.com/66228518/197652175-b1da0a63-fdcc-4fdd-bee8-557160cd0eea.JPG)

## Vista en Tableta - Página estática (/quienes-somos)
![quinesSomos-tablet](https://user-images.githubusercontent.com/66228518/197652253-2be3f5a8-9b89-492f-ac59-db385066459b.JPG)

## Vista en Teléfono - Página estática (/quienes-somos)
![quinesSomos-phone](https://user-images.githubusercontent.com/66228518/197652312-4966ff68-1698-414a-b022-76c543e1264d.JPG)

## Vista de Escritorio - Página estática (/cart)
Carrito vacío  
![cart-empty-desktop](https://user-images.githubusercontent.com/66228518/197653136-5e051305-b3e3-44e3-88ee-948a2bb75368.JPG)

Carrito con productos  
![cart-desktop](https://user-images.githubusercontent.com/66228518/197653143-f8b67cf9-42ef-402a-a822-57db81f746dd.JPG)

## Vista de móviles - Página estática (/cart)
Carrito vacío  
![cart-empty-mobile](https://user-images.githubusercontent.com/66228518/197653200-823a94e0-45fd-48cb-a7ca-9dca9504850f.JPG)

## Vista en Tableta - Página estática (/cart)
Carrito con productos  
![cart-tablet](https://user-images.githubusercontent.com/66228518/197653395-6e3f752d-9fce-47f2-bfa8-6385ff0df051.JPG)

## Vista en Teléfono - Página estática (/cart)
Carrito con productos  
![cart-phone](https://user-images.githubusercontent.com/66228518/197653450-329b22d0-f76f-4b62-b179-2622a81b0c40.JPG)

## Configuration

### Paso 1 - Configuración básica  
Ingrese a la [guía básica de configuración](https://developers.vtex.com/vtex-developer-docs/docs/vtex-io-documentation-2-basicsetuptodevelopinvtexio) de VTEX IO y siga los pasos.  
Al final de la configuración, debería tener instalada la interfaz de línea de comandos de VTEX (Toolbelt) junto con un workspace para desarrolladores en el que pueda trabajar.

### Paso 2 - Clonación del repositorio Minimum Boilerplate.

Use este repositorio como [plantilla](https://github.com/vtex-apps/minimum-boilerplate-theme) para crear un repositorio de forma local para poder comenzar a trabajar de manera efectiva en él

Luego, acceda al directorio del repositorio usando su terminal.

### Paso 3 - Editando el archivo Manifest.json
Una vez en el directorio del repositorio, es hora de editar el archivo manifest.json.

Una vez estemos en el archivo, deberá remplazar los valores de vendor y name. vendor es el nombre de la cuenta en la que estamos trabajando y account es lo que desee colocar de nombre para su tema. Opcionalmente puede modificar la versión  

Por ejemplo:  
{
  "vendor": "itgloberspartnercl",
  "name": "store-theme",
  "version": "0.0.1"
}

### Paso 4 - Instalando las apps requeridas
Para usar Store Framework y trabajar en el tema de su tienda, es necesario tener `vtex.store-sitemap` y `vtex.store` instalados.

Ejecute `vtex list` y compruebe si esas aplicaciones ya están instaladas.

Si no es así, ejecute el siguiente comando para instalarlos: `vtex install vtex.store-sitemap vtex.store -f`

### Paso 5 - Desinstalar cualquier tema existente
Al correr `vtex list`, puede verificar si hay algún tema instalado.

Es común tener ya instalado un vtex.store-theme cuando inicia el proceso de desarrollo front de la tienda.

Por lo tanto, si lo encuentra en la lista de la aplicación, copie su nombre y utilícelo junto con el comando `vtex uninstall`. Por ejemplo:

```json
vtex uninstall vtex.store-theme
```
### Paso 6 - Ejecute y obtenga una vista previa de su tienda
Entonces ha llegado el momento de cargar todos los cambios que realizó en sus archivos locales a la plataforma. Para eso, use el comando `vtex link`.

Si el proceso se ejecuta sin errores, se mostrará el siguiente mensaje: `App linked successfully`. Luego, ejecute el comando vtex browse para abrir una ventana del navegador con su tienda vinculada.

Esto le permitirá ver los cambios aplicados en tiempo real, a través de la cuenta y el espacio de trabajo en el que está trabajando.


## Dependencias  
1. Store minimun boilerplate theme  
2. Store GraphQl

## Store Component Apps  
1. "vtex.store": "2.x"  
2. "vtex.store-header": "2.x"  
3. "vtex.product-summary": "2.x"  
4. "vtex.store-footer": "2.x"  
5. "vtex.store-components": "3.x"  
6. "vtex.styleguide": "9.x"  
7. "vtex.slider": "0.x"  
8. "vtex.carousel": "2.x"  
9. "vtex.shelf": "1.x"  
10. "vtex.menu": "2.x"  
11. "vtex.minicart": "2.x"  
12. "vtex.product-details": "1.x"  
13. "vtex.product-kit": "1.x"  
14. "vtex.search-result": "3.x"  
15. "vtex.login": "2.x"  
16. "vtex.my-account": "1.x"  
17. "vtex.flex-layout": "0.x"  
18. "vtex.rich-text": "0.x"  
19. "vtex.store-drawer": "0.x"  
20. "vtex.locale-switcher": "0.x"  
21. "vtex.product-quantity": "1.x"  
22. "vtex.product-identifier": "0.x"  
23. "vtex.product-specification-badges": "0.x"  
24. "vtex.product-review-interfaces": "1.x"  
25. "vtex.telemarketing": "2.x"  
26. "vtex.order-placed": "2.x"  
27. "vtex.stack-layout": "0.x"  
28. "vtex.tab-layout": "0.x"  
29. "vtex.responsive-layout": "0.x"  
30. "vtex.slider-layout": "0.x"  
31. "vtex.iframe": "0.x"  
32. "vtex.breadcrumb": "1.x"  
33. "vtex.sticky-layout": "0.x"  
34. "vtex.add-to-cart-button": "0.x"  
35. "vtex.store-image": "0.x"  
36. "vtex.modal-layout": "0.x"  
37. "vtex.search": "2.x"  
38. "vtex.store-icons": "0.x"  
39. "vtex.checkout-summary": "0.x"  
40. "vtex.disclosure-layout": "1.x"  
41. "vtex.product-list": "0.x"  
42. "vtex.product-price": "1.x"  
43. "vtex.store-link": "0.x"  

## Dependencias Peer store component  
1. "vtex.reviews-and-ratings": "3.x"  
2. "vtex.wish-list": "1.x"  
3. "vtex.questions-and-answers": "0.x"  

## Custom Apps  
1. "itgloberspartnercl.whatsapp-button": "0.x"  
2. "itgloberspartnercl.bullets-diagramation": "0.x"  
3. "itgloberspartnercl.add-to-cart-info": "0.x"  
4. "itgloberspartnercl.custom-department-search": "0.x"  
5. "itgloberspartnercl.pdf-reader": "0.x"  
6. "itgloberspartnercl.quick-order": "0.x"  
7. "itgloberspartnercl.special-diagramation": "0.x"  

## Contributors  
1.	Luber María Cardona Vargas

